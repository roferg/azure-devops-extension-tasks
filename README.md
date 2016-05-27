# Build and Release Tasks for Team Services Extensions

Tasks to help you simplify and automate the delivery of Team Services extensions. Package, publish, share, and install your Team Services extensions to the Visual Studio Marketplace.

## Tasks included

* **Package**: package a Team Services extension into an extension package (.VSIX) file
* **Publish**: publish an extension (either privately or publicly) to the Visual Studio Marketplace
* **Share**: share an extension with a Team Services account
* **Install**: install an extension to a Team Services account
* **Query version**: query an extension's version (to make it easy to increment on your next package or publish)

## To use

After [installing the extension](https://marketplace.visualstudio.com/items?itemName=ms-devlabs.vsts-developer-tools-build-tasks) from the Marketplace, you can add one (or more) of the tasks to a new or existing [build definition](https://www.visualstudio.com/en-us/docs/build/define/create) or [release definition](https://www.visualstudio.com/en-us/docs/release/author-release-definition/more-release-definition)

![add-task](add-task.png)

If you plan to publish to the Marketplace, you will need to [create a personal access token](https://www.visualstudio.com/docs/setup-admin/team-services/use-personal-access-tokens-to-authenticate). 
 > **Important**: choose **All accessible accounts** and at least the **Marketplace (publish)** scope.

## To contribute

1. From the root of the repo run `npm run initdev`. This will pull down the necessary modules and TypeScript declare files.
2. Run `npm run build:tasks` to compile the build tasks
3. Run `npm run package:tasks` to create a .vsix extension package that includes the build tasks

