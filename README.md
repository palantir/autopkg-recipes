# autopkg-recipes

## About

This is a collection of AutoPkg recipes used to automate the process of packaging and deploying Mac applications.

## Usage

See [AutoPkg's documentation](https://github.com/autopkg/autopkg/wiki/Getting-Started) for instructions on using these recipes in your AutoPkg installation.

## Contributing

We welcome all contributions from the open source community to be submitted for review (in the form of GitHub pull requests). Feel free to fork this project and submit changes for approval. Thank you so much for taking the time to contribute!

## Shared AutoPkg Processors

The recipes in this repository make use of some third-party shared processors to accomplish workflows not included in the core AutoPkg product. The sections below include the source repository and documentation for each processor. To add these shared processors' repositories to AutoPkg, run `autopkg repo-add $repo` for each repo.

### AppIconExtractor

- Source: `haircut-recipes`
- Documentation: [Automatically Export and Generate App Icons in AutoPkg Recipes](https://macblog.org/autopkg-icons/)

Several .pkg recipes in this repo run the AppIconExtractor processor to prepare an icon file for use in recipe overrides, such as JamfUploader workflows.

### ExeVersionExtractor

- Source: `hansen-m-recipes`

1Password-Win.download.recipe runs this processor to determine the downloaded application version.

### JamfUploader

- Source: `grahampugh-recipes`
- Documentation: [JamfUploader wiki](https://github.com/grahampugh/jamf-upload/wiki/JamfUploader-AutoPkg-Processors)

The .jamf-upload recipes in this repo run the JamfPackageUploader and JamfCategoryUploader processors to upload a .pkg payload to Jamf along with its package category, but an override must be created for any additional JamfUploader actions, including creating or updating an associated policy.

### MSIVersionProvider

- Source: `hansen-m-recipes`
- Documentation: [Processors for Windows Software](https://github.com/autopkg/hansen-m-recipes/tree/master/SharedProcessors#msiinfoversionproviderpy)

Box-Win.download.recipe runs this processor to determine the downloaded application version.

### StringReplacer

- Source: `grahampugh-recipes`
- Documentation: [Common Processors](https://github.com/autopkg/grahampugh-recipes/tree/main/CommonProcessors#StringReplacer)

uTrust Common Driver.pkg.recipe runs this processor to convert the version string to a standard format.

### VariableFromPath

- Source: `magnusviri-recipes`
- Documentation: [AutoPkg notes](https://magnusviri.com/autopkg-notes.html)

uTrust Common Driver.pkg.recipe runs this processor to extract the version string from the downloaded file's name.

## Reference Links

### AutoPkg

[AutoPkg](https://autopkg.github.io/autopkg/) is a system for automatically preparing software for distribution to managed clients.

### MacAdmins Slack

[MacAdmins Slack](https://www.macadmins.org) is a great way to reach out for questions about Mac management and participate in the Mac admin community.

## License

This project is made available under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
