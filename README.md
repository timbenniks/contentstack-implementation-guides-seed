# Implementation Guides Stack Seed Content

This repository aims to provide sample stack content to users for the implementation of the implementation guides examples. An easy way to import this stack content is by using the seed command.

### Note : Contentstack stack must have English as Master Language

To import this content to your stack, perform the following steps:

1. Install the CLI by running the following command in your terminal:

```bash
npm i -g @contentstack/cli
```

2. By default, CLI uses the North America region. Based on where your Organization resides change this.
   To use the Europe region, run this command in your terminal:

```bash
csdx config:set:region EU
```

3. Next, log in to your Contentstack account via CLI:

```bash
csdx auth:login
```

4. Run the ‘seed’ command to import content to your stack:

```bash
csdx cm:stacks:seed --repo "timbenniks/contentstack-implementation-guides-seed" --org "<YOUR_ORG_ID>" -n "Implementation Guide"
```

Refer to the [Seed command documentation](https://www.contentstack.com/docs/developers/cli/import-content-using-the-seed-command/) to learn more.
