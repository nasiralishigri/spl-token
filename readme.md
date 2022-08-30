
#Generate Wallet 
solana-keygen new  --force -o "path set" // Create Wallet keys
solana-keygen pubkey // check publick key
solana balance --url devnet // check balance of account
solana airdrop 2 -url devnet

#Configiration
$ solana config get
$ solana config set --url https://api.devnet.solana.com
$ solana config set --keypair ${HOME}/new-keypair.json

#Airdrop
$ solana airdrop 1

#Create Token
$ spl-token create-token --url devnet // Create SPL Token
$ spl-token supply AQoKYV7tYpTrFZN6P5oUufbQKAUr9mNYGe1TTJC9wajM // Check total supply of token
$ spl-token create-account  "token-Address" --url devnet // Create Account For That 
$ spl-token balance AQoKYV7tYpTrFZN6P5oUufbQKAUr9mNYGe1TTJC9wajM // check balance of Token on that account
$ spl-token mint AQoKYV7tYpTrFZN6P5oUufbQKAUr9mNYGe1TTJC9wajM 100 // Mint new token
$ spl-token accounts // get all Token and Thier balance in specific account 
$spl-token authorize Cc3VqAGfiVYtxu4mauoxdzATY5pjqKR7D8dAX4awX2Rd mint --disable devnet // disable minting
$spl-token burn "Token Account " 100 --url devnet
