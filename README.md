# Action Repository

This repository is used only to **generate GitHub events** (push, pull request, merge)
for testing a GitHub Webhook receiver.

## Purpose
- Trigger `push`, `pull_request`, and `merge` events
- Acts as the **source repository**
- Does NOT contain backend or webhook code

## How it works
Any push or pull request made to this repository automatically triggers
a GitHub Webhook configured in the repository settings.

## How to trigger events

### Trigger PUSH
```bash
echo "test" >> test.txt
git add .
git commit -m "Trigger push event"
git push
