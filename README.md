# Verification Modal

## About

This repo contains the frontend code of the modal that receives authentication or verification configs and supports the flows by connecting users to the selected providers and completing a verification within your own system.

![image](https://github.com/walliDprotocol/verification-modal/assets/39834004/079ace06-141f-437f-beab-d33b1159ed68)

## How to use it

### 1. Create your config

Create a verification config with your own parameters based on digital IDs, DIDs, social IDs and blockchain assets using the libs in our [`core-config`](https://github.com/walliDprotocol/core-config) repo.

### 2. Launch Modal in your environment

#### Project setup

```
npm install
```

#### Compiles and hot-reloads for development

```
npm run serve
```

#### Compiles and minifies for production

```
npm run build
```

#### Lints and fixes files

```
npm run lint
```

#### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).

## Demo example

Check a live demo of the Modal with an example config in [`this website`](https://sdk-iframe.herokuapp.com/)

### Config parameters

The parameters provided are used for running an iframe within a suitable environment. Here is a description of each parameter:

PORT: This parameter specifies the port number on which the iframe will be hosted. It represents the network communication endpoint that the iframe will use to receive and send data.
PUBLISH_KEY: This parameter is related to PubNub, a real-time messaging service. The PUBLISH_KEY is a unique identifier or token that allows the iframe to publish messages or data to PubNub channels. It grants the necessary permissions to send information.
PUBNUB_SUBSCRIBE_KEY: This parameter is also associated with PubNub and represents another unique identifier or token. The SUBSCRIBE_KEY is used by the iframe to subscribe to PubNub channels, enabling it to receive messages or data from those channels.
PUBNUB_USER_ID: This parameter represents the user identification or identifier associated with the iframe in the PubNub system. It helps in distinguishing and tracking individual users or instances of the iframe within the messaging service.

These parameters are typically filled with specific values, such as actual port numbers, PubNub keys, and user IDs, which need to be provided according to the particular environment and requirements of the iframe setup.
