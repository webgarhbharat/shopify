# Shopify Theme Development

This repository contains a Shopify theme that can be developed and tested locally using the Shopify CLI.

## Prerequisites

Ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/) (latest LTS recommended)
- [Shopify CLI](https://shopify.dev/docs/themes/tools/cli/installation)
x
## Installation

To install the Shopify CLI globally, run the following command:

```sh
npm install -g @shopify/cli@latest
```

## Running the Theme Locally

To preview and develop your theme locally, use the following command:

```sh
shopify theme dev --store {store-name}
```

For example:

```sh
shopify theme dev --store=d926d1-a5.myshopify.com
```

This command will start a local development server and open a preview of your theme in the specified Shopify store.

## Additional Resources

For more information, visit the [Shopify Theme Development Documentation](https://shopify.dev/docs/themes).

---

**Note:** Ensure you have the necessary permissions to access and modify the store before running the development server.

Once you tested the theme locally you can push it the ther branch it will auto update to shopify 


## Professional Git Workflow Guide: Pushing and Pulling from a Branch

## Check Status
git status

## Verify Branch
git branch

## Pull Before Push
### Always pull the latest changes to avoid conflicts:
git pull origin staging
git push origin staging

## 1. Stage, commit
git add .

git commit -m "Your message"

## 2. Sync with remote
git pull origin staging

## 3. Push Code
git push origin staging


To pull the latest code from a Git repository without making any local changes, including commits, you can use the following command:

git pull --rebase


If you want to reset everything to match the remote branch exactly (discarding any local changes or commits), use:

git fetch origin
git reset --hard staging  # Replace 'main' with your branch name

git reset --hard origin/master

git rebase --abort