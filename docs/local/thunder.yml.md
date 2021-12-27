---
category: 2. Local Development Environment
order: 3
title: thunder.yml
description: The envionment configurations
permalink: /local-development/yaml
---

Your project directory will contain a YAML definition with contents that look like:

```yml
project:
    name: bookshelf
    git: https://git.thunder.so/cherry-blossom-1234.git
    directory: site
    env:
        - 
            name: local
            url: https://bookshelf.local
        -
            name: localtest
            url: https://bookshelf.local:8080
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
$ th update
Creating environment called production with branch main... done, ⬢ Creating cloudbits.io
https://cloudbits.io
``` 