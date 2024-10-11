# Implementation Guides Stack Seed Content

This repository aims to provide sample stack content to users for the implementation of the implementation guides examples. An easy way to import this stack content is by using the seed command.

> Contentstack stack must have English as Master Language

To import this content to your stack, perform the following steps:

### 1. Install the CLI

Install the CLI by running the following command in your terminal:

```bash
npm i -g @contentstack/cli
```

### 2. Set your region

By default, CLI uses the North America region. Based on where your Organization resides change this.
Run this command in your terminal (a list of options will show):

```bash
csdx config:set:region
```

### 3. Authenticate

Next, log in to your Contentstack account via CLI:

```bash
csdx auth:login
```

### 4. Seed your stack

To be able to seed a new Stack, find your Organization UID in Contentstack.

> Contentstack Stacks overview > Org Admin > Info

Run the `seed` command to import content to your stack (`-n` can be used for a custom Stack name):

```bash
csdx cm:stacks:seed --repo "timbenniks/contentstack-implementation-guides-seed" --org "<YOUR_ORG_UID>" -n "Implementation Guide"
```

Refer to the [Seed command documentation](https://www.contentstack.com/docs/developers/cli/import-content-using-the-seed-command/) to learn more.

## Additional info

This stack seed was exported like this from its origin. Follow the steps.

```bash
csdx cm:stacks:export
```
