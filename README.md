## Mantle Authorize.NET Integration

[![license](http://img.shields.io/badge/license-CC0%201.0%20Universal-blue.svg)](https://github.com/moqui/AuthorizeDotNet/blob/master/LICENSE.md)
[![release](http://img.shields.io/github/release/moqui/AuthorizeDotNet.svg)](https://github.com/moqui/AuthorizeDotNet/releases)

Moqui component for Authorize.Net AIM and CIM integrations that tie into Mantle payment processing and CIM integration to tokenize credit card information.

To add this component to Moqui the easiest approach is to use the Gradle get component task:

    $ ./gradlew getComponent -Pcomponent=AuthorizeDotNet

Or add a dependency in your component.xml file like:

    <depends-on name="AuthorizeDotNet"/>

To use simply:

1. load the demo configuration data in data/AuthorizeDotNetDemoData.xml or create your own configuration and load it; if you use the demo data, add the login and tranKey credentials
2. configure the store payment gateway with a ProductStorePaymentGateway record (see the demo data file for examples)
3. test the gateway with some test orders/payments
4. start receiving money...

The AIM and CIM payment services have been tested using the Mantle test scripts with the payment configuration in place as described above.
