# ![LOGO](logo.png) Numbers **flow**ground Connector

## Description

A generated **flow**ground connector for the Numbers API (version 2.0).

Generated from: https://api.apis.guru/v2/specs/whapi.com/numbers/2.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:53+03:00

## API Description

The William Hill Numbers API uses a single method that allows you to generate random numbers for your application. Numbers can either be unique or can be produced with the chance that some might be the same. For example, you can have a highest value of 6 and a lowest value of 1 with a count of 2 with a unique value of false - this will give you two numbers between 1 and 6 which are independent, just like two dice being rolled.<br /><br />The Numbers API is a Private API and therefore not automatically available to developers. To use this API, contact your business manager who will guide you through the separate Terms and Conditions of use before you can have the API assigned to your application.

## Authorization

Supported authorization schemes:
- API Key
## Actions

### This method is used to generate random numbers for your app. Within the request, you can specify the lowest number, the highest number and the amount of numbers returned. There is also an option to generate a unique set of numbers with no repetition of the same numbers allowed in the return.

*Tags:* `Numbers`

#### Input Parameters
* `apiSecret` - _required_ - Another unique identifier for your application. The secret must never be sent over HTTP.
* `apiTicket` - _optional_ - The authentication ticket associated with the user session. The getRandomNumbers method operates in two different ways - 'Demo' mode and 'Live' mode. In Demo mode, where no money is involved, the ticket is not required and can be used without it. In Live mode, when there is a financial outcome, the developer must supply a valid authentication and the ticket must be supplied. Important: The service should not be used in Live mode without a ticket.
* `gameCode` - _required_ - Identifier that indicates the game for which the RNG (Random Number Generator) has been used.
* `highest` - _required_ - Highest possible value to be returned.
* `lowest` - _required_ - Lowest possible value to be returned.
* `count` - _required_ - Number of values to be returned.
* `unique` - _required_ - Should the numbers returned be unique

## License

**flow**ground :- Telekom iPaaS / whapi-com-numbers-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
