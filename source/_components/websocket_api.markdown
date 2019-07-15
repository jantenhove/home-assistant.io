---
layout: page
title: "Websocket API"
description: "Instructions on how to setup the WebSocket API within Home Assistant."
date: 2018-01-21 08:00
sidebar: true
comments: false
sharing: true
footer: true
logo: home-assistant.png
ha_category:
  - "Other"
ha_qa_scale: internal
ha_release: 0.34
---

The `websocket_api` integration set up a WebSocket API and allows one to interact with a Home Assistant instance that is running headless. This integration depends on the [`http` component](/components/http/).

<div class='note warning'>

It is HIGHLY recommended that you set the `api_password`, especially if you are planning to expose your installation to the internet.

</div>

## Configuration

```yaml
# Example configuration.yaml entry
websocket_api:
```

For details to use the WebSocket API, please refer to the [WebSocket API documentation](/developers/websocket_api/) .

## Track current connections

The websocket API provides a sensor that will keep track of the number of current connected clients. You can add it by adding the following to your configuration:

```yaml
# Example configuration.yaml entry
sensor:
  platform: websocket_api
```
