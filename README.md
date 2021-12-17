# Attu

[![typescript](https://badges.aleen42.com/src/typescript.svg)](https://badges.aleen42.com/src/typescript.svg)
[![downloads](https://img.shields.io/docker/pulls/zilliz/attu)](https://img.shields.io/docker/pulls/zilliz/attu)
[![codecov](https://codecov.io/gh/zilliztech/attu/branch/main/graph/badge.svg?token=jvIEVF9IwW)](https://codecov.io/gh/zilliztech/attu)

Attu provides an intuitive and efficient GUI for Milvus, allowing you to interact with your databases and manage your data with just few clicks.

<img src="./.github/images/screenshot.png" alt="attu" />

## Attu Doc

- [English](./doc/en.md)
- [中文](./doc/zh-cn.md)

## Features and Roadmap

Attu is under rapid development and we are adding new features weekly, here are the current plan, we will release a version once a feature is available.

- Manage collections/partitions
- Manage index
- Basic statistics overview
- Load/release collections for search
- Insert entities
- Vector search with advanced filter
- System view
- Data view (TBD)
- View root node configuration(TBD)
- Vector Visualization(TBD)
- More...

## Quick start

### Before you start

Ensure you have Milvus installed on [your server](https://milvus.io/docs/install_standalone-docker.md) or [cluster](https://milvus.io/docs/install_cluster-docker.md), and attu only supports Milvus 2.x.

### ⭐️ Start a attu instance

```code
docker run -p 8000:3000 -e HOST_URL=http://{ attu ip }:8000 -e MILVUS_URL={milvus server ip}:19530 zilliz/attu:latest
```

Once you start the docker, open the browser, type `http://{ attu ip }:8000`, you can view the attu.

#### Params

| Parameter  | Example                 | required | description                       |
| :--------- | :---------------------- | :------: | --------------------------------- |
| HOST_URL   | http://192.168.0.1:8000 |   true   | Where attu container is installed |
| MILVUS_URL | 192.168.0.1:19530       |  false   | Optional, Milvus server URL       |

Tip: **127.0.0.1 or localhost will not work when runs on docker**

#### Try the dev build

**_note_** We plan to release attu once a feature is done. Also, if you want to try the nightly build, please pull the docker image with the `dev` tag.

```code
docker run -p 8000:3000 -e HOST_URL=http://{ your machine IP }:8000 -e MILVUS_URL={ your machine IP }:19530 zilliz/attu:dev
```

## ✨ Building and Running attu, and/or Contributing Code

You might want to build Attu locally to contribute some code, test out the latest features, or try
out an open PR:

### Build server

1. Fork and clone the repo
2. `cd server` go to the server directory
3. `yarn install` to install dependencies
4. Create a branch for your PR

### Build client

1. Fork and clone the repo
2. `cd client` go to the client directory
3. `yarn install` to install dependencies
4. Create a branch for your PR

### Milvus

New to milvus? Milvus is an open-source vector database built to power AI applications and embedding similarity search.

### Userful links

- [Milvus installation guide](https://milvus.io/docs/v2.0.0/install_standalone-docker.md)
- [Milvus python sdk](https://milvus.io/docs/v2.0.0/explore_pymilvus.md)
- [Milvus bootcamp](https://milvus.io/bootcamp)

#### ❓ Questions? Problems?

- If you've found a bug or want to request a feature, please create a [GitHub Issue](https://github.com/zilliztech/attu/issues/new/choose).
  Please check to make sure someone else hasn't already created an issue for the same topic.
- Need help using attu? Ask away on our [attu Discuss Forum](https://github.com/zilliztech/attu/discussions) and a fellow community member or
  Milvus engineer will be glad to help you out.

[milvus-doc]: https://milvus.io/docs/home

## Community

👉 Join the Milvus community on [Milvus forum](https://join.slack.com/t/milvusio/shared_invite/zt-e0u4qu3k-bI2GDNys3ZqX1YCJ9OM~GQ) to share your suggestions, advice, and questions with our engineering team.

<a href="https://join.slack.com/t/milvusio/shared_invite/zt-e0u4qu3k-bI2GDNys3ZqX1YCJ9OM~GQ">
    <img src="https://camo.githubusercontent.com/fa0663f8947e22e589e75ebbc84f0a835191d3ddab9a3a0f1dd054ef18eabbaa/68747470733a2f2f7a696c6c697a2d636d732e73332e75732d776573742d322e616d617a6f6e6177732e636f6d2f726561646d655f736c61636b5f346130376334633932662e706e67" alt="Miluvs Slack Channel"  height="150" width="500">
</a>
