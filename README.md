# **Raydium Pairs Volume Bot** ⚙️

This bot is designed to automate the distribution of SOL to multiple wallets and execute endless buy and sell swap transactions simultaneously on the **Raydium** platform. It leverages **Solana's** blockchain technology to perform these operations efficiently.

### *⚠️ Note: This product demonstrates the basic functions of a volume bot and is not suitable for large live tokens. For a more advanced version, please refer to [Version 2](#) on my GitHub.*

## **Features** ✨

- **💸 Automated SOL Distribution**: Distributes SOL to new wallets.
- **🔄 Endless Buy and Sell Swaps**: Simultaneously performs buy and sell transactions.
- **⚙️ Configurable Parameters**: Customizable buy amounts, intervals, distribution settings, and more.
- **💥 Massive Buy Mode**: Configure multiple wallets for large-scale buy operations.
- **📉 Sell Mode**: Gradually sells all tokens in sub-wallets through small transactions.
- **🔗 Token Pair Settings**: Configurable token mint and pool ID for swap operations.
- **📝 Logging**: Adjustable logging levels for improved monitoring and debugging.

## **Environment Variables** 🔐

The bot uses the following environment variables, which should be defined in a `.env` file:

![Solana](https://img.shields.io/badge/solana-%2300BFFF.svg?style=for-the-badge&logo=solana&logoColor=white) 
![Crypto](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=Crypto&logoColor=%23F7DF1E) 
![Node.js](https://img.shields.io/badge/node.js-%23339933.svg?style=for-the-badge&logo=node.js&logoColor=white) 
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) 
![npm](https://img.shields.io/badge/npm-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white) 
![Git](https://img.shields.io/badge/git-%23F05032.svg?style=for-the-badge&logo=git&logoColor=white) 





```env
PRIVATE_KEY=                 # Private key for the main wallet
RPC_ENDPOINT=                # RPC endpoint for Solana
RPC_WEBSOCKET_ENDPOINT=      # RPC WebSocket endpoint for Solana

####### BUY SETTING #######
IS_RANDOM=true               # Enable random buy amounts
DISTRIBUTION_AMOUNT=0.01     # Amount of SOL to distribute to each wallet
BUY_AMOUNT=0.01              # Fixed buy amount
BUY_UPPER_AMOUNT=0.002       # Upper limit for random buy amount
BUY_LOWER_AMOUNT=0.001       # Lower limit for random buy amount

BUY_INTERVAL_MAX=2000        # Maximum interval between buys in milliseconds
BUY_INTERVAL_MIN=4000        # Minimum interval between buys in milliseconds

CHECK_BAL_INTERVAL=3000      # Interval to check wallet balances in milliseconds
DISTRIBUTE_WALLET_NUM=8      # Number of wallets to distribute SOL to

SWAP_ROUTING=true            # Enable swap routing

###### FOR MASSIVE BUY #####
WALLET_NUM=8                 # Number of wallets for massive buy operations

########## FOR SELL MODE ##########
SELL_ALL_BY_TIMES=20         # Number of times to sell all tokens in sub-wallets gradually
SELL_PERCENT=100             # Percentage of tokens to sell from the main wallet

#### TOKEN PAIR SETTING ####
TOKEN_MINT=6VbEGuqwhjdgV9NxhMhvRkrFqXVNk53CvD7hK3C3yQS9  # Token mint address
POOL_ID=null                  # Pool ID for the token pair

TX_FEE=10                    # Transaction fee
ADDITIONAL_FEE=0.006         # Additional fee (should be larger than 0.006 SOL)
JITO_KEY=                    # Jito key
JITO_FEE=120000              # Jito fee
BLOCKENGINE_URL=ny.mainnet.block-engine.jito.wtf  # Block engine URL

###### GENERAL SETTING ######
LOG_LEVEL=info               # Logging level (info, debug, error)
```


## **Usage** 🤖

| Step | Command/Action                                                                                                      | Description                                                                                                      |
|------|---------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| 1    | ```git clone https://github.com/AlaMoonzzz/Solana-raydium-volume-bot.git```<br>```cd Raydium-Volume-Bot-Solana```  | 📂 **Clone** the repository and navigate to the bot directory.                                                   |
| 2    | ```npm install```                                                                                                   | 📦 **Install** the required dependencies.                                                                        |
| 3    | Rename the `.env.copy` file to `.env` and configure the environment variables.                                       | ⚙️ **Configure** RPC, WSS, main keypair's secret key, and jito auth keypair.                                     |
| 4    | ```npm start```                                                                                                     | 🚀 **Run** the bot.                                                                                              |


## **Author** ✍️

- **Telegram**: [https://t.me/AlaMoonzzz](https://t.me/AlaMoonzzz)
- **Discord**: [https://discord.com/users/304228787250528256](https://discord.com/users/304228787250528256)

You can always find me here for help or to discuss other projects. Feel free to reach out! 💬
