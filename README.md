# About
This is an example repository that demonstrates how to use the [CA API Gateway Developer Plugin][gateway-developer-plugin].

# Getting Started

## Building the Solution
In order to package the solution into something that can be applied to the CA API Gateway run the following Gradle command:

```gradle build```

This takes the solution that is contained in the `src/main/gateway` folder and packages it into a bundle at `build/gateway/zipped.bundle`

## Running the Solution
In order to run the solution you need to do the following:

1) Put a valid gateway license in the `docker` folder. The license file should be called `license.xml`
2) Make sure you have already built the solution by running `gradle build`
3) Start the Gateway Container by running: `docker-compose up`

After the container is up and running you can connect the CA API Gateway Policy Manager to it and/or call the example API at `/example`

## Exporting Updates
If you connect to the running gateway with the CA API Gateway Policy Manager and make changes to the services you can export those changes by running:

```gradle export```

This will export the changes to the `src/main/gateway` folder. Note that your local edits will be overridden by changes from the gateway

# About the Example Solution
The solution that is checked into this repository is contains a single folder and service. The service exposes `/example` and will respond with the following JSON for any HTTP(S) request:
```json
{
   "you-say": ["Hello", "Gateway"],
   "gateway-says": ["Hello", "User"]
}
```

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