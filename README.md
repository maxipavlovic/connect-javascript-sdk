# Connect Javascript SDK

CloudBlue Connect is a supply automation platform that manages your products and services, contracts, 
ordering and fulfillment, usage and subscriptions. 

It supports any product, from physical goods to cloud products, as well as any channel, including your 
direct and indirect sales channels and internal procurement. 

With its flexible APIs, it can connect to any commerce platform.

Vendors can leverage CloudBlue Connect to:

* Reduce the total cost of ownership for homegrown technology supporting their indirect channel
* Standardize integrations with partners
* Increase efficiencies and minimize redundancies by bridging their direct and indirect sales channels

Service providers can use CloudBlue Connect to:

* Define, manage and distribute any type of product (omni-product) through any channel (omni-channel)
* Transform perpetual licensed products into a subscription model
* Onboard new products into their portfolio quickly to build and deliver unique solutions to end customers


Connect Javascript SDK allows an easy and fast integration with the Cloud Blue Connect Platform. 
Thanks to it you can automate the fulfillment of orders generated by your products.



## Dependencies

Connect Javascript SDK work with Node.js version 8 or later.

Connect Javascript SDK also depends on:

* [lodash](https://lodash.com/) version 4.17.15
* [node-fetch](https://www.npmjs.com/package/node-fetch) version 2.6.0


## Install

To install the Connect Javascript SDK from a terminal window type:

```sh
$ npm install --save @cloudblueconnect/connect-javascript-sdk
```

## Documentation

The full SDK documentation is available [here](https://connect-javascript-sdk.readthedocs.io/).


## Usage

### Obtain the API endpoint and an API key

Before you start, you must obtain the API endpoint URL and an API key to access the Cloud Blue Connect Public API.

Go to your portal, from the navbar menu choose the `API` module.

In the `General` section you can find your API endpoint.

In the left side menu, choose `Tokens` to go to the API token view.

Once in the `Token` view, click on the button `CREATE TOKEN` on the upper right corner of the view.

### Example

```js

// import the ConnectClient class
const { ConnectClient } = require('@cloudblueconnect/connect-javascript-sdk');

// create an instance of the ConnectClient class
const client = new ConnectClient('https://<your api endpoint>/', '<your api key>');

// get a list of the latest version of publishd products
const products = await client.products.list();
```

## Contribute

If you want to contribute to the Connect Javascript SDK development feel free to open issues or fork the github repository and submit your pull request.


## License

The Connect Javascript SDK is licensed under the [*Apache License 2.0*](http://www.apache.org/licenses/LICENSE-2.0).


