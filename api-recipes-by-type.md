# API recipes by Type
\| [Browsing by Usecase](./api-recipes-by-usecase.md) \|  Browse by Type \|

* [API Proxies](#api-proxies)
* [Policy Templates](#policy-templates)
---
## API Proxies
[How to consume an API Proxy?](https://help.sap.com/viewer/66d066d903c2473f81ec33acfe2ccdb4/Cloud/en-US/9342a932441e45cd9636eb0a01a89958.html)

| Scenarios | Description | Usecase |
| --- | --- | --- |
| [Basic authenticatin to target endpoint](./authentication/basicauthentication) | Sample showcasing the generation of basic authentication header values for authentication with target endpoint. Edit the *setcredential* policy to provide the credentials to be used to connect to the target endpoint | [Authentication](#Authentication) |
| [SAML 2.0 browser profile based authentication to target endpoint](./authentication/saml) | Sample showcasing the handling of SAML 2.0 browser profile based authentication to the target endpoing using JavaScript policy | [Authentication](#Authentication) |
| [Basic authentication for user credentials, SAML 2.0 Browser Profile Authentication for Target Endpoint](./authentication/basictosamlauth) | Sample showcasing the enablement of an API proxy with basic authentication. The user name and password is passed in the HTTP header. Authorization is then used to trigger the SAML 2.0 browser profile flow to the target endpoint. | [Authentication](#Authentication) |
| [Cross-Origin Resource Sharing (CORS)](./cors) | Sample showcasing the handling of a response with a CORS header. This is helpful in scenarios where the targer server doesn't support sending CORS headers. | [Cross Origin Resource Sharing](#cors) |
| [Quota](./quota) | Sample showcasing the control the flow of traffic from the client to the target servers using *Quota* polices. It contains samples to limit the no of calls allowed per developer and also showcases quota violation handling using a HTTP 429 status as per the [RFC](https://tools.ietf.org/html/rfc6585#page-3) | [Traffic Management](#traffic) |
| [Spike Arrest](./spikearrest) | Sample showcasing the throttling of the number of incoming request processed by the API proxy. | [Traffic Management](#traffic) |
| [SQL Threat Protection](./sqlthreatprotection) | Sample showcasing the detection of SQL threats in a query parameters and error handling via HTTP 403 Forbidden response. | [Security](#security) |
| [Url Masking](./urlmask) | Sample showcasing the masking/rewriting of the target system host, basepath and replacing it with the proxy endpoint host and base path. | [Security](#security) |
| [Verify API Key](./verifyapikey) | Sample showcasing the enforcement and verification of API key based access to the API Proxy. Sample contains examples to pass the API key either as header parameter or as query parameter. | [Authentication](#Authentication) |

## Policy Templates
[How to consume a Policy Template?](./policy-templates/README.md)

Policy Template|Description|Usecase |
---|---| --- |
[API Management debugging and traceability](for/api-management-debugging-and-traceability)|Assists in API proxy execution performance assessment| [Debugging and Tracing](#debugging-and-tracing) |
[CORS](for/CORS)| Supports your API to be consumed by the application where CORS support is not available| [Cross Origin Resource Sharing](#cors)|
[Connect to SAP Cloud Foundry services](for/connect-to-sap-cloud-foundry-services)|Helps to manage mircoservices running in cloud foundry using SAP Cloud Platform API Management| [Consume APIs  of an Applications or Platform](#Connectivity) |
[Connect to SAP Cloud Platform services](for/connect-to-sap-cloud-platform-services)|Helps in consuming APIs hosted on SAP Cloud Platform and protected by Cloud Platform OAuth| [Consume APIs  of an Applications or Platform](#Connectivity) |
[Connect to SAP Concur](for/connect-to-sap-concur)|Facilitates easy consumption of Concur APIs protected by OAuth| [Consume APIs  of an Applications or Platform](#Connectivity) |
[Connect to SAP SuccessFactors](for/connect-to-sap-successfactors)| Helps to consume SAP SuccessFactors APIs protected by OAuth| [Consume APIs  of an Applications or Platform](#Connectivity) |
[JSON Threat Protection](for/json-threat-protection)|Assists you in securing your APIs from JSON threats for APIs managed by API Management| [Security](#security) |
[Metadata Cache for Odata APIs](for/metadata-cache-for-odata-apis)|Helps to improve performance of Odata API Proxies by caching metadata across invocations| [Caching](#caching) |
[Principal propagation via SAML](for/principal-propagation-via-saml)|Assists you in SAML User propagation from the application to back-end system via SAP API Management| [Authentication](#Authentication) |
[Quota With 429 Status Code](for/quota-with-429-status-code)|Helps to set quota and 429 status message| [Traffic Management](#traffic) |
[SQL Threat Protection](for/sql-threat-protection)|Assists you in securing your APIs from SQL threat for APIs managed by API Management| [Security](#security) |
[URL Masking](for/url-masking)|Assists in protecting backend system for APIs managed by API Management| [Security](#security) |
[Verify APIKey](for/verify-api-key)|Assists you in protecting APIs by Verifying the API Key | [Authentication](#Authentication) |
[XML Threat Protection](for/xml-threat-protection)|Protects APIs from XML threats for APIs managed by API Management| [Security](#security) |