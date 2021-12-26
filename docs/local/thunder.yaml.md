---
category: 2. Local Development Environment
order: 3
title: thunder.yaml
description: The envionment configurations
permalink: /installation/yaml
---

Your project directory will contain a YAML definition with contents that look like:

```yaml 
project:
    name: bookshelf
    git: https://git.thunder.so/cherry-blossom-1234.git
    directory: site
    env:
        - 
            name: local
            url: https://bookshelf.local
        -
            name: staging
            url: https://cherry-blossom-1234.thunderapp.com
            branch: staging
            volumes:
                - web/app/uploads:bucket-cherry-blossom-1234
        -
            name: production
            url: https://cloudbits.io
            branch: main

```

To sync infrastructure with the definition, run:

```sh
th project update
Creating environment called production with branch main... done, ⬢ Creating cloudbits.io
https://cloudbits.io
``` 