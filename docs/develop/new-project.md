---
category: 2. Develop
order: 2
title: Local Development Environment
description: New Local WordPress development environment based on Docker
permalink: /develop/
---

Create new project with Thunder.

```bash
$ th new bookshelf
New project created at `bookshelf` directory.
New Git repository provisioned: https://git.thunder.so/cherry-blossom-1234.git
Cloning Bedrock
Run composer within Bedrock directory
2200 files successfully created

You are ready to install Wordpress here: https://bookshelf.local
```

This will provision a local website ```https://bookshelf.local``` within the ```~/Documents/www/bookshelf``` directory.


List the projects known by Thunder on your computer.

```bash
$ th list projects
```

Use Docker compose command to start new project. Ensure Docker Desktop is operational.

```bash
$ cd bookshelf
$ docker compose up -d
```

Perform your changes locally and update your repository.

```bash
$ git add . && git commit -m "Initial commit"
```