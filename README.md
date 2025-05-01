# autopkg-recipes

## About

This is a collection of AutoPkg recipes used to automate the process of packaging and deploying Mac applications.

## Usage

See [AutoPkg's documentation](https://github.com/autopkg/autopkg/wiki/Getting-Started) for instructions on using these recipes in your AutoPkg installation.

## Contributing

We welcome all contributions from the open source community to be submitted for review (in the form of GitHub pull requests). Feel free to fork this project and submit changes for approval. Thank you so much for taking the time to contribute!

## Reference Links

### AutoPkg

[AutoPkg](https://autopkg.github.io/autopkg/) is a system for automatically preparing software for distribution to managed clients.

### JamfUploader

The .jamf-upload recipes in this repo run the JamfPackageUploader processor written by Graham Pugh to upload a .pkg payload to Jamf (as well as its package category), but an override must be created for any additional JamfUploader actions, including creating or updating an associated policy.. Running recipe overrides of these recipes will require adding JamfUploader's repository to AutoPkg by running `autopkg repo-add grahampugh-recipes`. See the [JamfUploader wiki](https://github.com/grahampugh/jamf-upload/wiki/JamfUploader-AutoPkg-Processors#using-the-processors) for more information on using this family of processors in your recipes.

### AppIconExtractor

Several .pkg recipes in this repo run the AppIconExtractor processor written by Matthew Warren to prepare an icon file for use in recipe overrides, such as JamfUploader workflows. Running recipe overrides of these recipes will require adding AppIconExtractor's repository to AutoPkg by running `autopkg repo-add haircut-recipes`. See [Automatically Export and Generate App Icons in AutoPkg Recipes](https://macblog.org/autopkg-icons/) for more information on using this processor in your recipes.

### MacAdmins Slack

[MacAdmins Slack](https://www.macadmins.org) is a great way to reach out for questions about Mac management and participate in the Mac admin community.

## License
This project is made available under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
