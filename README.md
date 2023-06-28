# backstage-export

This repository contains exported data from API Hub for a 
[Backstage](https://backstage.io) developer portal application.

## Generating the export

The data in the `apigee-apihub-demo` folder is generated using the experimental
`registry-connect` CLI command housed in the
[registry-experimental](https://github.com/apigee/registry-experimental) repo.

Example:

```sh
curl -L https://raw.githubusercontent.com/apigee/registry-experimental/main/downloadLatest.sh | sh -
export PATH=$PATH:$HOME/.registry/bin
registry-connect publish backstage apigee-apihub-demo --owner-name "API Hub Demo" --owner-desc "API Hub Demo"
```

## Viewing the data

Follow the instructions in the
[backstage-example](https://github.com/apigee-apihub-demo/registry-experimental) repo
to start and access the example Backstage app.

## Disclaimer

This demonstration is not an officially supported Google product.

## License

Unless otherwise specified, all content is owned by Google, LLC and released
with the Apache license.
