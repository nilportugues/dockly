<img width="200" src="https://user-images.githubusercontent.com/316371/28937414-67ee5ffa-7893-11e7-95f9-5059cacf9170.png">

[![view on npm](http://img.shields.io/npm/v/dockly.svg)](https://www.npmjs.org/package/dockly)
[![view on npm](http://img.shields.io/npm/l/dockly.svg)](https://www.npmjs.org/package/dockly)
[![npm module downloads](http://img.shields.io/npm/dt/dockly.svg)](https://www.npmjs.org/package/dockly)
[![Dependency Status](https://david-dm.org/lirantal/dockly.svg)](https://david-dm.org/lirantal/dockly)
[![Codefresh build status]( https://g.codefresh.io/api/badges/build?repoOwner=lirantal&repoName=dockly&branch=master&pipelineName=dockly&accountName=lirantal&type=cf-1)]( https://g.codefresh.io/repositories/lirantal/dockly/builds?filter=trigger:build;branch:master;service:58127ed36b0e230100f421f6~dockly)

🌟 Featured on [![Awesome Docker](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/veggiemonk/awesome-docker) [![DevOps Weekly](https://img.shields.io/badge/DevOpsWeekly-%F0%9F%95%B6-yellow.svg
)](http://devopsweekly.com) 



# Dockly
Docker console UI and Dashboard for quick manging and inspecting of Containers and Images

![dockly-demo-2](https://cloud.githubusercontent.com/assets/316371/25682867/c5212216-3027-11e7-8f36-72d38516d2af.gif)

# Install
Install the API module as a depdency in your project so you can easily use it to query Operations Orchestration REST API

```javascript
npm install -g dockly
```

# Usage

Just fire up dockly and it will automatically connect to your localhost docker daemon through the unix socket:

```
dockly
```

## Command line options:

It's also possible to provide command line options for dockly to customize the docker connection

| Param | Type | Description |
| --- | --- | --- |
| -h or --host | string | Docker host to connect to |
| -p or --port | string | Docker port to connect to |
| -s or --socketPath | string | Docker socket to connect to |

# Docker Support

## Build
You can build dockly as a docker image yourself, using the following command:

```
docker build -t dockly .
```

## Run
To run dockly as a container, invoke the following command:

```
docker run -it --name dockly -v /var/run/docker.sock:/var/run/docker.sock dockly
```

# Author
Liran Tal <liran.tal@gmail.com>
