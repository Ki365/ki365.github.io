+++
title = 'Terminology'
date = 2024-07-04T00:19:41-06:00
draft = false
comments = false
weight = 3
+++

## Introduction

Ki365 repackages many existing concepts into distinctive terminology. To become familiar with how Ki365 is used, refer to the following documentation.

## Concepts

### Data Owners

Organizations or individuals who use Ki365 are considered data owners.

### Project Storage

Ki365 serves a slim internal git repository as primary project storage. This serves two purposes:

- Redundancy
- Availability

When a project is connected to Ki365, the repository is always fully stored on the Ki365 instance. This ensures Ki365 users always have their project data.

Further information on the types of project storage is found in the Project Connections section below.

### Project Connections

Projects are added to Ki365 through Project Connections. These connections allow flexibility and simplicity of data storage depending on how the data owner wants to store their data.

#### Link

Linked repositories are the most flexible type of project connection. They allow data owners to submit changes to the Ki365 and have them forwarded to the linked data store as a form of offsite backup. This type of connection combines the simplicity of a local connection and the resiliency of a mirrored type.

{{<callout type="info">}}
If using this connection type, please ensure commit messages are properly signed and enforced. Otherwise, ownership of changes can easily be spoofed.
{{</callout>}}

#### Mirror

Mirrored repositories are projects which are direct copies of remote data stores outside Ki365 control. They are read only and require data owners to submit changes to the remote data store. Ki365 is subject to either api data limits and access restrictions on public/private repositories.

{{<callout emoji="🌐">}}
Only use this type of connection if Ki365 storage use is not desired. All other Ki365 features relating to data stored per project on Ki365 can be configured under the Admin settings on the application web portal.
{{</callout>}}

#### Local

Local repositories are stored in a local git server and backed up to the internal data store (see backup section for more information)

{{<callout type="warning">}}
Even though this is a convent project connection, it is the most vulnerable to data loss. Only choose this option backup is enabled or if the data is not critical.
{{</callout>}}

###
