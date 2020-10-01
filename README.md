# About
This is an example repository that demonstrates how to use [API Gateway Policy Plugin.](https://techdocs.broadcom.com/content/broadcom/techdocs/us/en/ca-enterprise-software/layer7-api-management/gateway-policy-plugin/1-0.html)

<!---

# About
This is an example repository that demonstrates how to use the [CA API Gateway Developer Plugin][gateway-developer-plugin].

# Getting Started

## Building the Solution
In order to package the solution into something that can be applied to the CA API Gateway run the following Gradle command:

```./gradlew build```

## Running the Solution
In order to run the solution you need to do the following:

1) Put a valid gateway license in the `docker` folder. The license file should be called `license.xml`. For information on getting a license see the [License Section from the Gateway Container readme](https://hub.docker.com/r/caapim/gateway/).
2) Make sure you have already built the solution by running `./gradlew build`
3) Start the Gateway Container by running: `docker-compose up`

After the container is up and running you can connect the CA API Gateway Policy Manager to it.

## Exporting Updates
If you connect to the running gateway with the CA API Gateway Policy Manager and make changes to the services and policies you can export those changes by running:

```./gradlew export```

This will export the changes to the various project folders. Note that your local edits will be overridden by changes from the gateway

# Giving Back
## How You Can Contribute
Contributions are welcome and much appreciated. To learn more, see the [Contribution Guidelines][contributing].

## License

Copyright (c) 2018 CA. All rights reserved.

This software may be modified and distributed under the terms
of the MIT license. See the [LICENSE][license-link] file for details.


 [license-link]: /LICENSE
 [contributing]: /CONTRIBUTING.md
 [gateway-developer-plugin]: https://github.com/ca-api-gateway/gateway-developer-plugin
--->
