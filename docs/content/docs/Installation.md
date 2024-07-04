+++
title = 'Installation'
date = 2024-07-01T20:16:28-06:00
draft = false
comments = false
weight = 1
+++

Ki365 is a modern web application. As such, the installation process involves several industry standard tools for standing up a server instance:

- A terminal (command prompt) interface
- [Docker compose](https://www.docker.com/)
- [Git Source Code Manager (SCM)](https://git-scm.com/)

To install a Ki365 instance:

{{% steps %}}

### Step 1

Navigate to the computer terminal which will host Ki365.

{{<callout type="info">}}
A common computer operating system for servers is [Ubuntu Server LTS](https://ubuntu.com/server).
{{</callout>}}

### Step 2

Ensure docker compose is installed, run:

```
docker compose version
```

### Step 3

Install the application by running:

```
git clone --depth 1 https://github.com/Ki365/Ki365.git
cd Ki365
docker compose up
```

{{% /steps %}}

### Shutting Down

To shutdown Ki365, run the following in the same Ki365 directory from above:

```
docker compose down
```
