---
category: 3. Deploy
order: 2
title: New Environment
description: An overview of IaC concepts and philosophy
permalink: /deploy/new-env
---

Churn up new environments on demand using any branch of code.

```bash
$ thunder env create testing --branch=nightly
Creating environment called tesing with branch nightly ... done, ⬢ Creating ambidextrous-susan-1234
https://ambidextrous-susan-1234.thunderapp.com/
```

The above code would add the following to the ```thunder.yml``` dcoument in your project directory.

```yml
        -
            name: testing
            url: https://ambidextrous-susan-1234.thunderapp.com/
            branch: nightly
```