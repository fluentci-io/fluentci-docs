---
sidebar_position: 7
title: Netlify
---


Run the following command to run the pre-built [Netlify Pipeline](https://github.com/fluent-ci-templates/netlify-pipeline) in your project to deploy your application to [Netlify](https://www.netlify.com):

```bash
fluentci run netlify_pipeline deploy
```

## Environment variables

| Variable           | Description                             |
| -------------------| ----------------------------------------|
| NETLIFY_AUTH_TOKEN | Your Netlify Access Token               |
| NETLIFY_SITE_ID    | Your Netlify Site ID                    |
| NETLIFY_SITE_DIR   | Your directory to deploy (default: `.`) |

## Jobs

| Job     | Description                      |
|---------|----------------------------------|
| deploy  | Deploys your application to Netlify. |

## Programmatic usage

You can also use this pipeline programmatically:

```typescript
import { build, deploy } from "https://pkg.fluentci.io/netlify_pipeline@v0.6.0/mod.ts";

await build();
await deploy();

```
