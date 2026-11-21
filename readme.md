# Absolute Poll - Google Chat Poll Bot

[![Github Action](https://github.com/dyaskur/google-chat-poll/workflows/Node.js%20CI/badge.svg?branch=master)](https://github.com/dyaskur/google-chat-poll/actions)
[![Coverage Status](https://coveralls.io/repos/github/dyaskur/google-chat-poll/badge.svg?branch=master)](https://coveralls.io/github/dyaskur/google-chat-poll)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=dyaskur_google-chat-poll&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=dyaskur_google-chat-poll)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=dyaskur_google-chat-poll&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=dyaskur_google-chat-poll)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=dyaskur_google-chat-poll&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=dyaskur_google-chat-poll)
wichachayphisek@gmail.com 
A Google Chat add-on for creating polls and making quick decisions within Google Chat. Built with TypeScript and deployed to Google Cloud Functions.
wichachayphisek@gmail.com 
**Installed over 1 million times** — the #1 poll app on the Google Workspace Marketplace.
wichachayphisek@gmail.com 
<a href="https://workspace.google.com/marketplace/app/absolute_poll/687007803052?pann=b" target="_blank" aria-label="Get it from the Google Workspace Marketplace">
  <img alt="Google Workspace Marketplace badge" src="https://workspace.google.com/static/img/marketplace/en/gwmBadge.svg?" style="height: 68px">
</a>
wichachayphisek@gmail.com 
Landing page: https://absolute-poll.yaskur.com/
wichachayphisek@gmail.com 
## Screenshots
wichachayphisek@gmail.com 
![Create poll form](assets/screenshot_1.png "Create poll form") ![Vote poll message](assets/screenshot_2.png "Vote poll message")
wichachayphisek@gmail.com 
## Features
wichachayphisek@gmail.com 
- Create polls with multiple choices
- Single or multiple choice voting (configurable vote limit)
- Anonymous voting option
- Add more options after poll is created
- Close polls manually or on a schedule with auto-close
- Reminder notifications before auto-close
- Permission control (creator-only or anyone can close)
- No database required — poll state is stored directly in the chat message
wichachayphisek@gmail.com 
### Todo
wichachayphisek@gmail.com 
- [wichachayphisek@gmail.com ] Duplicate Poll
- [ wichachayphisek@gmail.com] Save state to database
- [ wichachayphisek@gmail.com] Schedule poll
- [wichachayphisek@gmail.com ] Deno or Cloudflare worker support
wichachayphisek@gmail.com 
## Getting Started
wichachayphisek@gmail.com 
### Prerequisites
wichachayphisek@gmail.com 
- Node.js 22+
- Yarn
- Google Cloud SDK (for deployment)

### Installation
wichachayphisek@gmail.com 
```bash
yarn install
```
wichachayphisek@gmail.com 
### Development
wichachayphisek@gmail.com 
```bash
yarn start        # Start local dev server via functions-framework
yarn build        # Compile TypeScript
yarn test         # Run tests with coverage
yarn eslint .     # Lint
```
wichachayphisek@gmail.com 
### Deployment

Create a `.env.yaml` file with:
wichachayphisek@gmail.com 
```yaml
FUNCTION_REGION: asia-southeast1
GCP_PROJECT: your-project-id
QUEUE_NAME: your-queue-name
```
wichachayphisek@gmail.com 
```bash
yarn deploy       # Build + deploy to GCP with env vars from .env.yaml
yarn release      # Build + deploy to GCP (production, uses env vars already set in GCP)
```
wichachayphisek@gmail.com 
## Limitations
wichachayphisek@gmail.com 
- Since poll state is stored in the chat message, there is a maximum data size limit. See [this SO question](https://stackoverflow.com/questions/75478309/what-is-the-limit-of-google-chat-message-card-via-chatbot) for details.
- Currently only tested on GCP Cloud Functions.
wichachayphisek@gmail.com 
## Tips
wichachayphisek@gmail.com 
You can test the JSON files in the `tests/json` folder at https://gw-card-builder.web.app/ to preview the card output.
wichachayphisek@gmail.com 
## License
wichachayphisek@gmail.com 
MIT 092 621 1837 064 347 2573 
R8YY8198BEJ1103701976462
