# Simple Capacitor/Trapeze Example

Simple overview of common uses for [Trapeze](https://trapeze.dev/).

## Description

This is a simple example of using Trapeze Config Tool to edit your native projects in a Capacitor-based project.

## Getting Started

### Dependencies

* [Installing the Trapeze Config Tool](https://trapeze.dev/docs/configuration-tool)
* `npm install @trapezedev/configure`

### Usage

Two `scripts` were added that will update both the pacakage/bundle identifier and application names for both iOS and Android for dev and production environments

```json
"trapeze:dev": "npx trapeze run trapeze.config.development.yaml -y",
"trapeze:prod": "npx trapeze run trapeze.config.production.yaml -y"
```

* `npm run trapeze:dev`: App will be named `[DEV] My App` with an bundle id of `io.ionic.starter.dev`
* `npm run trapeze:prod`: App will be named `My App` with an bundle id of `io.ionic.starter`
* Both can be installed on a device at the same time due to the unique bundle id

### Notes

* You can integrate this as needed with your build process. For example, check out [Capacitor CLI Hooks](https://capacitorjs.com/docs/cli/hooks)
* [Trapeze Configuration Docs](https://trapeze.dev/docs/configuration-tool)
* [Trapeze Project API Docs](https://trapeze.dev/docs/project-api) - This wasn't used in this example, but it's another potential option
