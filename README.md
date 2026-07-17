[![StepSecurity Maintained Action](https://raw.githubusercontent.com/step-security/maintained-actions-assets/main/assets/maintained-action-banner.png)](https://docs.stepsecurity.io/actions/stepsecurity-maintained-actions)

# Swift Package Registry

The [Swift Package Registry](https://swiftpackageregistry.com/) is a collection of Swift Packages. Since the [GitHub Swift Package Registry](https://github.blog/2019-06-03-github-package-registry-will-support-swift-packages/) is not currently released and the [IBM Swift Package Catalog](https://developer.ibm.com/swift/2016/02/22/introducing-swift-package-catalog/) is has been killed, the [Swift Package Registry](https://swiftpackageregistry.com/) fills the current gap for easier searching and discoverability of Swift Packages.

## Technical

This [GitHub App](https://developer.github.com/apps/about-apps/) is a [Node.js](https://nodejs.org/en/) application built with [Probot](https://github.com/probot/probot). It parses all Swift packages using [Docker](https://github.com/apocas/dockerode).

Only public repositories are supported. When adding packages manually, a personal access token is used to fetch information about the package. 

Docker is used to help validate packages. Just parsing <samp>Package.swift</samp> is not always enough. It is also an additional check for Swift version compatability.

You can access the [Swift Package Registry](https://swiftpackageregistry.com/) via [swiftpackageregistry.com](https://swiftpackageregistry.com/) (main site), [swift-packages.com](https://swift-packages.com), [swiftpkg.dev](https://swiftpkg.dev), and [swiftdependencies.com](https://swiftdependencies.com).

