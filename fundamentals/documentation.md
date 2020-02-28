---

copyright:
  years: 2019
lastupdated: "2019-11-06"

subcollection: sdk-handbook

---

# Documentation

## Interface documentation

The SDK MUST have accompanying documentation that clearly describes all public methods and classes of the SDK.
This includes full documentation for method parameters and responses and all member variables of classes.

The interface documentation SHOULD use terminology that is appropriate
for the programming language (e.g. Java objects should not be described as "JSON", and methods for
service invocations should not be described as a "GET /v3/path/to/the/service").

## Delivery format

SDK interface documentation SHOULD be integrated into the [IBM Cloud API Reference](https://cloud.ibm.com/apidocs) for the service,
where the SDK for each language appears in a separate tab.
See the [adding SDK content](/docs/developing/api?topic=api-docs-sdk-info) section of the
IBM Cloud API Docs tutorials for information on how to create and publish this documentation.

SDK interface documentation SHOULD also be delivered in a format and location that experienced developers
for a particular language / platform will find familiar
- Javadoc for a Java SDK
- [TypeDoc](https://typedoc.org/api/index.html) for a Node SDK
- [Sphinx](http://www.sphinx-doc.org/en/master/) for a Python SDK
- ? for a Go SDK
- Jazzy for a Swift SDK

## Tutorials and user guides

Tutorials and user guides for the service SHOULD provide prominent references to the SDK.
This should include how the SDK can be accessed through the package management systems appropriate for each language
and how this can be automated in a DevOps pipeline flow for an application using the SDK.

## Migration guides

Your SDK SHOULD provide a migration guide to help users upgrade to the latest version of your SDK.

## Examples

The SDK MUST include or have accompanying examples that illustrate common usage flows involving multiple service APIs.

All IBM-developed coding examples and sample applications for the service SHOULD use the SDK.

## Contributor documentation

The SDK MUST include documentation for developers that would like to contribute to the SDK
either by opening issues or submitting pull requests.

In particular:

### Issue template and pull request template

Provide issue and pull request templates to guide contributors on what information should be provided
and what processes to follow when making contributions to the SDK.

### CONTRIBUTING.md

Provide a CONTRIBUTING.md file in the root of the SDK repo containing the following information:
- The coding style established for the SDK. This is typically a reference to an externally documented coding
style for the language, with perhaps some exceptions specific to the SDK.
- How to build the SDK
- How to run the code style checker and use the autofix feature if available
- How to run the unit tests and integration tests
- How to run a single test (for debugging)
- How to run the code coverage tooling