---
category: 2. Develop
order: 4
title: Import Database
description: Import SQL database into Docker container
permalink: /develop/import-database/
---

```sh
# Run wp-cli commands
$ th exec wp 

# Import a database
$ th exec wp db import database-file.sql
Success: Imported from 'database-file.sql'
```

Use Wordpress [CLI Commands](https://developer.wordpress.org/cli/commands/) for reference.
