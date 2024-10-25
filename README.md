# Phrase Bridge Bot

A bot that posts phrases to Telegram channels using OpenAI API. The bot reads instructions from markdown files and generates content using OpenAI's GPT models, then posts the generated content to specified Telegram channels.

## Environment Variables

Create a `.env` using `.env.example` file.

## Installation

```bash
# Install dependencies
yarn install
```

## Usage

### Local Development

Run the bot locally:
```bash
yarn start
```

### Deploying to AWS Lambda

1. Build the package:
```bash
yarn deploy:package
```

2. Upload the generated ZIP file from `build/phrase-bridge-bot-[version].zip` to AWS Lambda
3. Configure environment variables in Lambda console
4. Set appropriate timeout and memory settings

## Scripts

- `yarn start` - Run the bot locally
- `yarn clean` - Clean build directories
- `yarn build:prod` - Create production build
- `yarn zip` - Create deployment archive
- `yarn deploy:package` - Full production build and packaging
