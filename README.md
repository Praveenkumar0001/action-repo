# action-repo

This repository demonstrates GitHub Actions and webhook integration.

## Features
- Triggers webhook on Push, Pull Request, and Merge events
- Sends event data to a registered endpoint (see webhook-repo)

## Setup
1. Fork or clone this repository.
2. Configure the webhook endpoint in `.github/workflows/webhook.yml` by replacing `<WEBHOOK_ENDPOINT>` with your actual endpoint URL.
3. Push changes or open pull requests to trigger events.

## Related
- See `webhook-repo` for the Flask/MongoDB endpoint implementation.
