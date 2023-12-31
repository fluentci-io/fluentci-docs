---
sidebar_position: 8
title: PHP
---


## Running the pre-built PHP pipeline directly

Run the following command to run the pre-built [PHP pipeline](https://github.com/fluent-ci-templates/php-pipeline) without having to initialize a project:

```bash
fluentci run php_pipeline
```

## Add PHP Pipeline to your project

Run the following command to add PHP pipeline to your project:

```bash
fluentci init -t php
```

This will create a `.fluentci` directory in your project, feel free to customize the pipeline for your needs.
You can then run the following command to start the pipeline:

```bash
fluentci run .
```

Or simply:

```bash
fluentci
```


## Environment variables

| Variable               | Description                                | Default |
| ---------------------- | ------------------------------------------ | ------------- |
|`MARIADB_USER`          | The username for the MariaDB database      | `homestead`        |
|`MARIADB_PASSWORD`      | The password for the MariaDB database      | `secret`    |
|`MARIADB_ROOT_PASSWORD` | The root password for the MariaDB database | `root`        |

## Jobs

| Job   | Description      |
| ----- | ---------------- |
| test  | Run your tests   |

## Programmatic usage

You can also use this pipeline programmatically:

```ts
import { test } from "https://pkg.fluentci.io/php_pipeline@v0.4.0/mod.ts";

await test();
```
