# Manipulate Excel Files in PHP 🐘

Code examples for the tutorial for the tutorial [How to Read and Write Excel Files in PHP](https://www.nidup.io/blog/manipulate-excel-files-in-php)

The code is packaged as a simple Symfony application with cli commands.

## Installation 📦

Download the source code:

```
git clone git@github.com:nidup/manipulate-excel-data-in-php.git
cd manipulate-excel-data-in-php
```

Then the installation comes into 2 flavors, directly on your host or using docker.

Once installed the commands are the same, some docker shortcuts are provided in `.docker/bin`.

### Install directly on your system (option A) 💻

Install the PHP dependencies:

```
composer install
```

### Install with docker & docker-compose (option B) 🐋

Build the docker image and install the PHP dependencies:

```
docker-compose up -d 
.docker/bin/composer install
```

## Use the console commands 🚀

Use `bin/console` or `.docker/bin/console` to launch a command.

List the commands:
```
bin/console --env=prod
[...]
nidup:excel-league:read-big-excel-file        Read a big excel file and measure time and memory (with box/spout)
nidup:excel-spout:generate-big-excel-file     Generate a 1M lines excel file (with box/spout)
nidup:excel-spout:read-excel-file             Read an excel file (with box/spout)
nidup:excel-spout:write-excel-file            Write an excel file (with box/spout)
[...]
```

Launch a command:
```
bin/console nidup:excel-spout:read-excel-file --env=prod
```

We use the prod environment here to have the most efficient execution.
