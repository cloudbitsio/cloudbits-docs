---
category: 3. Deploy
order: 2
title: New Environment
description: An overview of IaC concepts and philosophy
permalink: /deploy/new-env
---

```bash
thunder project env:create testing --branch=nightly
Creating environment called tesing with branch nightly ... done, ⬢ Creating ambidextrous-susan-1234
https://ambidextrous-susan-1234.thunderapp.com/
```

```yaml
        -
            name: testing
            url: https://ambidextrous-susan-1234.thunderapp.com/
            branch: nightly
```