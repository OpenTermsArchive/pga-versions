# Dataset PGA v2 (Ongoing Collection)

This dataset PGA v2 is part of the [Platform Governance Archive (PGA)](https://www.platformgovernancearchive.org/). It is the result of a continuous data collection of policies of up to 18 (social) media platforms since April 2022, performed with the [Open Terms Archive engine](https://docs.opentermsarchive.org/), and hosted and curated by the [Lab Platform Governance, Media And Technology (PGMT)](https://platform-governance.org/) at ZeMKI, University of Bremen. The PGA v2 dataset contains a selected set of policies for each platform that usually includes community guidelines, privacy policies and terms of service agreements. A number of platforms have more complex structures for laying out their rules, so PGA v2, for instance, tracks seven specific policies for TikTok and nine for Twitter. 

- **Platforms**: Facebook, Instagram, LINE, LinkedIn, Parler, Pintest, Quora, Reddit, Snapchat, Spotify, Telegram, TikTok, Tumblr, Twitch, Twitter, WeChat, WhatsApp, YouTube
- **Time Frame**: since April 2022 (most platforms)
- **Project Website:** [https://platformgovernancearchive.org](https://platformgovernancearchive.org)

## Background

This dataset PGA v2 is part of the [Platform Governance Archive (PGA)](https://www.platformgovernancearchive.org/), a data repository and platform that collects and curates policies of major social media platforms in a long-term perspective. In addition to PGA v2, there is also the [historical dataset PGA v1](https://github.com/PlatformGovernanceArchive/pga-corpus) that provides a long-term collection of platform policies of four major platforms from 2005 to 2021. The PGA v2 picks up this work and writes it into the future, while also broadening the scope of data collection. Instead of looking backward, the PGA v2 entails data collected in-real time as changes are made to platform policies. This way, the database remains always up to date allowing access to the data through the Platform Governance Archive even for the most current versions of platform policies. 

## Data Collection

The data collection is performed with the [Open Terms Archive engine](https://docs.opentermsarchive.org/). Open Terms Archive (OTA) is a French NGO focussed on making company terms and their changes available to consumers and the public, and offering an almost real-time alert service for such changes. The dataset PGA v2 utilizes the open source software, the Open Terms Archive Engine to download and archive changes of 18 platforms. Two aspects for data collection are important and linked to the OTA. The OTA Engine automatically updates the archive of the English language version of selected platform policies on a regular basis, capturing all meaningful edits in terms and policies. This is done by using an automated web scraper that tracks the changes of each web URL. The relevant parts of platform policies are selected [here](https://github.com/OpenTermsArchive/pga-declarations) with the use of CSS selectors and Javascript filters, to select the correct content, remove insignificant content (e.g. ads, illustrative pictures, internal navigation links…), and filter out noise (e.g. tracker identifiers in links, relative dates…). The engine scrapes through the selected policies multiple times a day, and keeps all HTML snapshots [here](https://github.com/OpenTermsArchive/pga-snapshots). If changes are detected within the HTML snapshots, new versions of the policy are populated to [PGA v2 dataset](https://github.com/OpenTermsArchive/pga-versions). Please consult the [documentation](https://docs.opentermsarchive.org/) for more information on the Open Terms Archive Engine.

Even when taking an automated approach, we could not archive all platforms this way. Going beyond the four platforms of PGA v1, we selected a total of 18 platforms to monitor for PGA v2. The logic for archiving decisions has largely been based on scale i.e. selecting the platforms with the largest possible usership. Since we were interested in social media platforms and not in commercial retail platforms such as Amazon or news websites that allow for comments under published articles. A number of these platforms can be best described as “chat services” although they might have a number of additional features. The sampling decision was made in early 2022 and usership numbers vary over time. For instance, the use of Parler has since strongly declined. Another sampling criterion is that the location of the platforms must be in the jurisdiction of the European Union (at least through a form of representation or agent). 

## Explore and Download the Data 

The data is organised by platforms, each having a dedicated folder in this repository. Within this folder, you find a markdown-file for each policy / document of this platform that we are tracking. For each of these files the repository includes the full history of changes. 

If you just want to work with the **current versions** of platform policies you can just click through the services and documents. You can also download the files in their current form by clicking on the green "Code" button on the top right and then "Download ZIP".

If you want to **explore the history of changes,** open the folder of the service of your choice. You will see the set of documents tracked for that service, now click on the document of your choice. For example, [YouTube's Community Guidelines](https://github.com/OpenTermsArchive/pga-versions/blob/main/YouTube/Community%20Guidelines.md). The latest version will be displayed. To view the history of changes made to this document, click on "History" at the top right of the document. The changes are ordered ante-chronologically (see [example](https://github.com/OpenTermsArchive/pga-versions/commits/main/YouTube/Community%20Guidelines.md)).

Click on a change to see its contents. The red colour shows deleted elements and the green colour shows added elements. For example, here is an interesting change in [YouTube's Community Guidelines](https://github.com/OpenTermsArchive/pga-versions/commit/30e6af989d9b8656fddad0dbb4086b2efa3e3a0c).

You can choose from two types of display with the icons in the grey bar above the document:

- The first one, named *source diff* (button with chevrons) displays the previous version and the next one [side by side](https://github.com/OpenTermsArchive/contrib-versions/commit/58a1d2ae4187a3260ac58f3f3c7dcd3aeacaebcd#diff-e8bdae8692561f60aeac9d27a55e84fc).
- The second one, named *rich diff* (button with a document icon) displays all the changes [in a single document](https://github.com/OpenTermsArchive/contrib-versions/commit/58a1d2ae4187a3260ac58f3f3c7dcd3aeacaebcd?short_path=e8bdae8#diff-e8bdae8692561f60aeac9d27a55e84fc). In this view, beyond green and red, the yellow color shows modified paragraphs. Be careful, this display does not show some changes such as hyperlinks and text style’s changes.

You can download the full repository including all tracked platforms and document with their complete history under "[Releases](https://github.com/OpenTermsArchive/pga-versions/releases)".

## Using the Data in your own Projects

We are more than happy if you want to use our dataset in your research, reporting, and explorations. If you do:

1. Consult the respective data documentation;
2. reference this project and the actual dataset;
3. send us a note so that we include you in our research and output page.

PGA v2 is made available under the [Open Data Commons Attribution License](http://opendatacommons.org/licenses/by/1.0/) (that means what we say above: use it, but reference us).

**Recommended Citation for Dataset** 
Katzenbach, C., Dergachava, D., Fischer, A., Kopps, A., Kolesnikov, S., Redeker. D., Viejo Otero, P. (2023). Platform Governance Archive (PGA): Dataset PGA v2. https://doi.org/10.26092/elib/2373.

**Recommind Citation for Single Policy Document**
Name of platform. (Date of version). Name of policy. *Platform Governance Archive*. Direct URL.


## Use RSS feed

You can receive notification for a specific service or document by subscribing to RSS feeds.

> An RSS feed is a type of web page that contains information about the latest content published by a website, such as the date of publication and the address where you can view it. When this resource is updated, a feed reader app automatically notifies you and you can see the update.

To find out the address of the RSS feed you want to subscribe to:

1. [Navigate](https://github.com/OpenTermsArchive/pga-versions#exploring-the-versions-history) to the page with the history of changes you are interested in. *In the OpenTermsArchive example above, this would be [this page](https://github.com/OpenTermsArchive/pga-versions/commits/main/OpenTermsArchive/Privacy Policy.md).*
2. Copy the address of that page from your browser’s address bar. *In the OpenTermsArchive example, this would be `https://github.com/OpenTermsArchive/pga-versions/commits/main/OpenTermsArchive/Privacy%20Policy.md`.*
3. Append `.atom` at the end of this address. *In the OpenTermsArchive example, this would become `https://github.com/OpenTermsArchive/pga-versions/commits/main/OpenTermsArchive/Privacy%20Policy.md.atom`.*
4. Subscribe your RSS feed reader to the resulting address.

#### Recap of available RSS feeds

| Updated for                    | URL                                                          |
| ------------------------------ | ------------------------------------------------------------ |
| all services and documents     | `https://github.com/OpenTermsArchive/pga-versions/commits.atom` |
| all the documents of a service | Replace `$serviceId` with the service ID: `https://github.com/OpenTermsArchive/pga-versions/commits/main/$serviceId.atom.` |
| One specific document          | Replace `$serviceId` with the service ID and `$documentType` with the document type: `https://github.com/OpenTermsArchive/pga-versions/commits/main/$serviceId/$documentType.md.atom` |

For example:

- To receive all updates of `Facebook` documents, the URL is `https://github.com/OpenTermsArchive/pga-versions/commits/main/Facebook.atom`.
- To receive all updates of the `Privacy Policy` from `Google`, the URL is `https://github.com/OpenTermsArchive/pga-versions/commits/main/Google/Privacy%20Policy.md.atom`.
