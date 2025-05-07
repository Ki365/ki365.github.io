+++
title = 'Installation'
date = 2024-07-01T20:16:28-06:00
draft = false
comments = false
weight = 1
+++

Ki365 is a modern web application designed to help people collaborate on their designs.

The installation process of this program requires a few industry standard tools:
- A CLI (command line interface) terminal
- A host computer which meets the [requirements](../requirements)
- A decent internet connection

To install Ki365:

{{% steps %}}

### Step 1

Navigate to the computer terminal which will host Ki365. This can be done through SSH.

{{<callout type="warning">}}
It is practically required to provision a server with access to at least 8Gb of RAM. Ki365 relies on a KiCad Docker container instance which has this requirement. 
{{</callout>}}

{{<callout type="info">}}
It is not recommended to rely on SWAP space for extending the virtual memory. This may cause long processing times after each commit of a project. 
{{</callout>}}

### Step 2

Install the application:

```
git clone --depth 1 https://github.com/Ki365/Ki365.git
cd Ki365
```

### (Optional) Step 3

Install the demo projects:
```
task setup
```

### Step 4

Start the instance:
```
docker compose start
```

{{% /steps %}}

### Shutting Down

To shutdown Ki365, run the following in the same Ki365 directory from above:

```
docker compose stop
```
