# Open Terms Archive - ${instanceName} versions

This repository is to be considered as a database only.
You can find the documentation by following the link in the “About” section of this page.

## How to use this template

This is a template for the `versions` repository of [Open Terms Archive](https://opentermsarchive.org)

**NOTE**: When creating from this template, please keep the naming structure of `${instanceName}-versions` in order to keep consistency across repos and organisations. 

In order to use it, follow this simple steps:
- Navigate to https://github.com/OpenTermsArchive/template-versions
- Click on `Use this template`
- Enter the name of the target repository `${instanceName}-versions` and the target organization
- Edit this file by clicking on the ![Edit Button](https://raw.githubusercontent.com/primer/octicons/main/icons/pencil-24.svg "Look, on the right of the title README.md") icon at the top right of this file *(This icon is visible if you have the right to modify this repo)*
- Remove this paragraph, change the ${instanceName} in the title and add any documentation you find necesary

You can also check the complete doc: [How to use a template on Github](https://docs.github.com/en/github-ae@latest/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

## Use RSS feed

You can receive notification for a specific service or document by subscribing to RSS feeds.

> An RSS feed is a type of web page that contains information about the latest content published by a website, such as the date of publication and the address where you can view it. When this resource is updated, a feed reader app automatically notifies you and you can see the update.

To find out the address of the RSS feed you want to subscribe to:

1. [Navigate](#exploring-the-versions-history) to the page with the history of changes you are interested in. _In the OpenTermsArchive example above, this would be [this page](https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/OpenTermsArchive/Privacy%20Policy.md)._
2. Copy the address of that page from your browser’s address bar. _In the OpenTermsArchive example, this would be `https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/OpenTermsArchive/Privacy%20Policy.md`._
3. Append `.atom` at the end of this address. _In the OpenTermsArchive example, this would become `https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/OpenTermsArchive/Privacy%20Policy.md.atom`._
4. Subscribe your RSS feed reader to the resulting address.

#### Recap of available RSS feeds

| Updated for                         | URL                                                                                                                                                                                            |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| all services and documents          | `https://github.com/OpenTermsArchive/${instanceName}-versions/commits.atom`                                                                                                                            |
| all the documents of a service      | Replace `$serviceId` with the service ID:<br>`https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/$serviceId.atom.`                                                            |
| One specific document               | Replace `$serviceId` with the service ID and `$documentType` with the document type:<br>`https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/$serviceId/$documentType.md.atom` |

For example:

- To receive all updates of `Facebook` documents, the URL is `https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/Facebook.atom`.
- To receive all updates of the `Privacy Policy` from `Google`, the URL is `https://github.com/OpenTermsArchive/${instanceName}-versions/commits/main/Google/Privacy%20Policy.md.atom`.


# License

Data in this repository is distributed under an ODC-BY 1.0 license. That means you are free to share (to copy, distribute and use the database), to create (to produce works from the database), to adapt (to modify, transform and build upon the database) as long as you attribute the resulting works to _Open Terms Archive with contributions from ${instanceMaintainer}_.

Contact the author if you have any specific need or question regarding licensing.
