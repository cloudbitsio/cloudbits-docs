---
category: 3. Deploy
order: 3
title: Sync Static Files
description: Sync uploads directory with S3 bucket
permalink: /deploy/sync
---

Synchronise the `uploads` directory using the command

```sh
th sync uploads <source> <destination>

Example usage:
th sync uploads local staging --verbose
```



Synchronise database:

```sh
th sync db <source> <destination>

Example usage:
th sync db local staging
You are about to push a local database to the cloud. Are you sure (Y/N): Y
Syncing database from local to staging... done.
```
