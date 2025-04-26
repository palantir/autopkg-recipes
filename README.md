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
A collection of Autopkg processors used for all the .jamf-upload recipes in this repository. Note that [using JamfUploader](https://github.com/grahampugh/jamf-upload/wiki/JamfUploader-AutoPkg-Processors#using-the-processors) requires adding the `grahampugh-recipes` repo to your AutoPkg preferences. The .jamf-upload recipes in this repo will upload the package to Jamf Pro (as well as its package category), but an override must be created for any additional JamfUploader actions, including creating or updating an associated policy.

### MacAdmins Slack
[MacAdmins Slack](https://www.macadmins.org) is a great way to reach out for questions about Mac management and participate in the Mac admin community.

## License
This project is made available under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
