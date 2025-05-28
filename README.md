# KiteAI Auto Bot

An automated bot for interacting with KiteAI testnet, performing daily tasks, and maximizing rewards.

## Features ✨

- **Automated Interactions**: Chat with KiteAI agents (Professor, Crypto Buddy, Sherlock)
- **Daily Faucet Claim**: Automatically claim daily KITE tokens
- **Staking System**: Stake tokens and claim rewards automatically
- **Multi-Wallet Support**: Manage multiple wallets simultaneously
- **Smart Analytics**: Track XP points, staking info, and rewards
- **Scheduled Execution**: Runs daily with countdown timer

## Prerequisites 📋

- Node.js v16+
- Ethereum wallet private key(s)
- [2Captcha API key](https://2captcha.com/?from=23248152) (for faucet claims)
- KiteAI testnet access https://testnet.gokite.ai?referralCode=S86CD815

## Installation ⚙️

1. Clone the repository:
```bash
git clone https://github.com/vikitoshi/KiteAI-Auto-Bot.git
cd KiteAI-Auto-Bot
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file based on `.env.example`:
```env
PRIVATE_KEY_1=your_private_key_here
# Add more wallets as needed
```

## Configuration ⚙️

Edit the `prompt.txt` file to customize your agent interactions. Format:
```
[Professor]
What is the future of AI in blockchain?
Explain neural networks like I'm five.

[Crypto Buddy]
Best crypto to invest in 2024?
How does DeFi work?

[Sherlock]
Solve this crypto mystery...
Analyze this transaction pattern
```

## Usage 🚀

Run the bot:
```bash
node index.js
```

The bot will:
1. Login with your wallet(s)
2. Display profile information
3. Claim daily faucet (if 2Captcha key provided)
4. Stake tokens and claim rewards
5. Interact with all agents using random prompts
6. Schedule next run in 24 hours

## Wallet Setup 💰

1. Get testnet ETH from a faucet
2. Get initial KITE tokens from the [KiteAI faucet](https://testnet.gokite.ai)
3. Stake at least 1 KITE token to start earning rewards

## Troubleshooting 🛠️

Common issues:
- `Invalid private key`: Ensure your private key starts with '0x'
- `reCAPTCHA errors`: Verify your 2Captcha API key and balance

## Security 🔒

- Never share your private keys
- Use environment variables for sensitive data
- The bot only interacts with official KiteAI endpoints
- Code is open for audit

## Contribution 🤝

Pull requests are welcome! For major changes, please open an issue first.

## Disclaimer ⚠️

This is an unofficial tool for educational purposes only. Use at your own risk. The developers are not responsible for any losses.

## License 📜

MIT
