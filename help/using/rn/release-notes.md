---
solution: Journey Optimizer
product: journey optimizer
title: Release notes
description: Journey Optimizer Release notes
exl-id: 06fa956a-b500-416e-9d42-b683c328e837
---
# Release notes {#release-notes}

[!DNL Adobe Journey Optimizer] continuously delivers new features, enhancements to existing features, and bug fixes. All changes are consolidated on the last week of each month in these release notes. 

Previous release notes are available in [this page](release-notes-2022.md). You can also consult the [latest documentation updates](documentation-updates.md) page for more changes.

[!DNL Adobe Journey Optimizer] is built natively on [!DNL Adobe Experience Platform] and inherits from its latest innovations and improvements. Learn more about these changes in [Adobe Experience Platform Release Notes](https://experienceleague.adobe.com/docs/experience-platform/release-notes/latest.html){target="_blank"}.

![Newsletter](../assets/do-not-localize/nl-icon.png) Sign up for the [Adobe Journey Optimizer quarterly newsletter](https://www.adobe.com/subscription/Adobe_Journey_Optimizer_NL.html){target="_blank"} today, and receive the latest product updates, exciting stories, use cases, tips and more delivered directly to your inbox every quarter.



## June 2023 release notes {#june-rn-2023}

<!--
Information below is subject to change without prior notice until the release availability date. Updated documentation will be published at the release date, and direct links will be added in this page.

**Release date**: June 21-22, 2023-->


<!-- ### New capabilities{#june-2023-features}-->

<table>
<thead>
<tr>
<th><strong>API-triggered campaigns for marketing use cases</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use APIs to trigger marketing campaigns in Adobe Journey Optimizer from an external system.</p>
<p>Until this release, API-triggered campaigns capability was covering various operational and transactional messaging needs like password resets or OTP token, but could not be used to create marketing campaigns. Available channels for API-triggered campaigns are: Email, SMS and Push messages.</p>
<img src="assets/do-not-localize/api-triggered.gif"/>
<p>For more information, refer to the <a href="../campaigns/api-triggered-campaigns.md">detailed documentation</a>.
</td>
</tr>
</tbody>
</table>

<!--
### Improvements {#june-2023-improvements}


**Audiences**

Enhancements have been made to the audience picker in journeys or campaigns, with the addition of new columns displaying the origin and update frequency of audiences.

**Journeys**

You can now leverage API call responses in custom actions and orchestrate your journey based on these responses.
-->

## May 2023 release notes {#may-rn-2023}

### New capabilities{#may-2023-features}

<!--
<table>
<thead>
<tr>
<th><strong>Audience Composition</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create composition workflows to combine existing Adobe Experience Platform audiences into a visual canvas and leverage various activities (split, enrich...) to create new audiences. Newly created audiences are saved backed into Adobe Experience Platform along with existing audiences and can be leveraged in Journey Optimizer campaigns to target customers.</p>
<img src="../segment/assets/audiences-publish.png"/>
<!--p>For more information, refer to the <a href="../offers/ranking/personalized-optimization-model.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

<table>
<thead>
<tr>
<th><strong>Content Experimentation in campaigns</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Journey Optimizer now supports experiments in campaigns. Experiments are randomized trials, which in the context of online testing, means that you expose some randomly selected users to a given variation of a message, and another randomly selected set of users to some other variation or treatment. After exposure, you can then measure the outcome metrics you are interested in, such as opens of emails, subscriptions, or purchases.</p>
<img src="assets/do-not-localize/experiment.gif"/>
<p>For more information, refer to the <a href="../campaigns/content-experiment.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Objective reporting and performance measurement in campaigns</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now measure the performance of your campaigns across inbound and outbound through dedicated reports. Adobe Journey Optimizer reports can retrieve additional metrics to use in the Objectives tab of your campaign reports.</p>
<img src="assets/do-not-localize/performance_report.gif"/>
<p>For more information, refer to the <a href="../reports/campaign-global-report.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->


<table>
<thead>
<tr>
<th><strong>Create and use fragments in your email content</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now author, use, and manage fragments to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Journey Optimizer campaigns and journeys for an improved and accelerated design process.</p>
<img src="assets/do-not-localize/fragments.gif"/>
<p>For more information, refer to the <a href="../email/fragments.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Use Tags in your campaigns (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now assign Adobe Experience Platform Unified Tags to your campaigns. This allows you to easily classify them and improve search from the campaigns list. Note that Unified tags feature is currently in beta.</p>
<img src="assets/do-not-localize/campaigns-tag.gif"/>
<p>For more information, refer to the <a href="../start/search-filter-categorize.md#tags">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>



<table>
<thead>
<tr>
<th><strong>Personalized Optimization AI ranking model (General Availability)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Personalized Optimization AI ranking models are now generally available in Decision Management. This new type of model allows you to optimize and personalize offers based on segments and offer performance.</p>
<img src="assets/do-not-localize/ai-ranking.gif"/>
<p>For more information, refer to the <a href="../offers/ranking/personalized-optimization-model.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>



### Improvements {#may-2023-improvements}

**Audiences**

* In preparation for the generally availability of the Audience Portal feature, Adobe Experience Platform is updating the usage of "audiences" and "segment" within the system and the documentation.

    * Audience: A set of people, accounts, households, or other entities that share common characteristics and behaviors.
    * Segment definition: In Adobe Experience Platform, the rules used to describe key characteristics or behavior of a target audience. This term was formerly known just as "segment".

    As a result, within Adobe Journey Optimizer and the Adobe Experience Platform UI, you'll see "Segments" replaced with "Audiences" to reflect this new path of audience creation and management.

    The translations of the term "audience" when referring to a group of profiles targeted to receive a message were harmonized across all Digital Experience products for some languages:
   
   * German: Zielgruppe
   * Brazilian Portuguese: público-alvo
   * Spanish: público destinatario

<!--* Enhancements have been made to the audience picker in journeys or campaigns, with the addition of new columns displaying the origin and update frequency of audiences.-->

**SMS channel**

* Infobip has been added as a vendor provider when configuring your SMS channel surfaces. [Read more](../sms/sms-configuration.md)
* Twillio - API credential setup now includes the ability to add Messaging service SID for seamless integration with your Twilio account. [Read more](../sms/sms-configuration.md)

**In-app channel**

* Added new message trigger rules for Adobe Places Service. [Read more](../in-app/inapp-configuration.md)
* Added new Adobe Experience Platform Assurance capabilities to capture device events to add as trigger rules.

<!--
**Journeys**

* You can now leverage API call responses in custom actions and orchestrate your journey based on these responses.
-->

**Campaigns**

* It is now possible to duplicate a campaign from the inventory screen using the ellipsis action menu. [Read more](../campaigns/modify-stop-campaign.md#duplicate)
* You can now delete draft modifications to a Live campaign.
* The steps for activating a campaign have now been streamlined. [Read more](../campaigns/modify-stop-campaign.md)

**Decision Management**

* You can now edit the frequency capping if the offer has the **[!UICONTROL Draft]** status and was never published before with frequency capping enabled. [Read more](../offers/offer-library/add-constraints.md#frequency-capping)

**Personalization**

* You can now select and insert asset references directly from Personalization Editor when working in HTML content.

### Fixes{#may-2023-fixes}

* In-App Messages – Fixed an issue where campaign scheduling conflicted with message frequency settings.


## April 2023 release notes {#apr-rn-2023}

<!--Information below is subject to change without prior notice until the release availability date. Updated documentation will be published at the release date, and direct links will be added in this page.

**Release date**: April 27, 2023-->

### New capabilities{#apr-2023-features}

<table>
<thead>
<tr>
<th><strong>Web channel (General Availability)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Journey Optimizer is expanding its cross-channel capabilities by adding support for web channel. You can now author, change, and preview web experiences as any other channel, through a smart and intuitive visual interface to personalize your end-users experience. Note that currently in Journey Optimizer you can only create web experiences in campaigns.</p>
<img src="assets/do-not-localize/web-authoring.gif"/>
<p>For more information, refer to the <a href="../web/get-started-web.md">detailed documentation</a>.</p>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Mobile onboarding quick start workflow (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The new mobile onboarding quick start workflow is now available. Use this new product feature to rapidly configure the Mobile SDK to start collecting and validating mobile event data, and send mobile push notifications with Adobe Journey Optimizer. This capability is accessible via the Data Collection home page as a public beta.</p>
<img src="../push/assets/mobile-wf-home.png"/>
<p>For more information, refer to the <a href="../push/mobile-onboarding-wf.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>New Journey dashboard (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p> The Journey dashboard is now split in two tabs:</p>
<ul><li>Use the <strong>Overview</strong> tab to access a new dashboard which displays key metrics related to your journeys.</li>
<li>Use the <strong>Browse</strong> tab to access the list of all journeys.</li></ul>
<p>This capability is accessible in all journeys as a public beta.</p>
<img src="assets/do-not-localize/journey-dashboard.gif"/>
<p>For more information, refer to the <a href="../building-journeys/journey-gs.md#journey-access">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#april-2023-improvements}

**Journeys**

* The journey canvas now displays the activity ID on message activities and end tags. This improves reporting and retargeting.
* The layout of the configuration pane, which appears in actions, data sources, events and journeys, has been improved.
* New insight to number of nodes on canvas with safeguards for helping grow: keep journeys easy to read, QA and troubleshoot with a maximum number of nodes per journey at 50. [Read more](../start/guardrails.md#journeys-guardrails-journeys)
* When adding an [Email](../email/create-email.md), [SMS](../sms/create-sms.md) or [Push](../push/create-push.md) action in a journey, the surface is now pre-filled, by default, with the last used surface for that channel, in the current journey.
* You can now define static or dynamic query parameters in your custom actions. [Learn more](../action/about-custom-action-configuration.md#url-configuration)

**Reporting**

* You can now export Journey Optimizer reports as PDF. [Learn more](../reports/global-report.md#export-reports)

**Content Designer**

* The Adobe Journey Optimizer Content Designer has been updated, and access to design styles and components is now easier. This new version propose an improved user experience, and comes with increased performances, dark mode partial compatibility, and new accessibility standards support.



## March 2023 release notes {#mar-2023}

### New capabilities{#mar-2023-features}

<table>
<thead>
<tr>
<th><strong>In-app channel (General Availability)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send personalized In-app messages to your app users within a campaign. Use Journey Optimizer to design notifications and customize the message layout, display, text, and buttons to create a seamless experience.</p>
<img src="assets/do-not-localize/in-app.gif"/>
<p>For more information, refer to the <a href="../in-app/get-started-in-app.md">detailed documentation</a>.</p>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>SMS click tracking</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>With SMS click tracking, you can monitor the performance of your shortened URLs, identify who clicked on them, and use this data to retarget those customers with subsequent campaigns.</p>
<img src="assets/do-not-localize/sms-tracking.gif"/>
<p>For more information, refer to the <a href="../sms/create-sms.md#sms-content">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Use Tags in your Journeys (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>As a Journey Optimizer practitioner, you can now organize your business objects using tags. Tags are a quick and easy way of classifying objects to improve search. This feature is currently in beta and only available for Journeys.</p>
<p>For more information, refer to the <a href="../start/search-filter-categorize.md#tags">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#mar-2023-improvements}

**Journeys**

* The new **Throttling API** allows you to set a limit on the number of events sent per second, preventing overwhelming traffic spikes on your external systems or API. When the set limit is reached, all subsequent API calls are queued and processed as soon as possible, in the order they were received. Please note that this feature supports only one throttling configuration across all your sandboxes. [Learn more](../configuration/external-systems.md)
* The Journey canvas has been enhanced for a simpler and improved user experience. At the end of each path in the canvas, the empty place holders have been removed. You can now simply add your activities by dragging them at the end of a path.
* In the journey canvas, the label of the **End** tag is no longer automatically set with the previous activity's name. Users can manually add a custom label if needed.
* The default timeout and error duration in journey properties has been changed from 5 to 30 seconds. [Learn more](../configuration/external-systems.md#timeout)
* The default throttling rate in read segment activities has been changed from 20,000 to 5,000 messages per second. [Learn more](../building-journeys/read-segment.md#configuring-segment-trigger-activity)
* A guardrail has been added to the test mode to only listen to events sent through the interface. Events send through an external tool are not taken into account. [Learn more](../building-journeys/testing-the-journey.md)


<!-- 
* When adding an Email, SMS or Push action in a journey, the surface is now pre-filled, by default, with the last used surface for that channel.
* A new type of system alert has been introduced. You can now get notified when a custom action fails. [Learn more](../reports/alerts.md)
* Timeout and error management has been improved in journeys. Timeout and error paths are now always added on the canvas. A new toolbar button is available to show/hide these paths. [Learn more](../building-journeys/journey-gs.md#timeout_and_error)
* The Journey dashboard is now split in two tabs:
    * Use the **Overview** tab to access a new dashboard which displays key metrics related to your journeys.
    * Use the **Browse** tab to access list of all journeys.
-->

**Decision management**

* To prevent any potential confusion with the recent release of tags feature across  Adobe Experience Platform, Decision Management tags have been renamed to "Collection qualifiers".

    Note that although the term "tag" is no longer used in Decision management user interface, it is still used in backend services such as APIs and datasets.

* You can now reset the offer capping counter on a daily, weekly or monthly basis. [Learn more](../offers/offer-library/add-constraints.md#capping)

* You can also choose which Adobe Experience Platform event should be looked at for offer decisioning capping. [Learn more](../offers/offer-library/add-constraints.md#capping)

* Additional parameters have been added in placements creation screen. They allow you to control whether an offer can be duplicated across multiple placements, and to specify if the offer's content and metadata should be included in the API response. [Learn more](../offers/offer-library/creating-placements.md)

**Personalization**

* You can now include default fallback text for string-based profile attributes in the Expression Editor. These values will display if the selected attributes return no result. [Learn more](../personalization/personalization-build-expressions.md#add)

**Reporting**

* The reporting widget functionality has been improved with the ability to customize how users view their data. With this improvement, users can now choose between multiple visualization options, including graph, table, and donut charts.

    To have access to the latest widgets, please note that you will have to reset the different reporting dashboards. For more information on dashboard customization, refer to the [detailed documentation](../reports/global-report.md#modify-dashboard).

## February 2023 release notes {#feb-2023}

### New capabilities{#feb-2023-features}

<table>
<thead>
<tr>
<th><strong>In-app channel (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send personalized In-app messages to your app users within a campaign. Use Journey Optimizer to design notifications and customize the message layout, display, text, and buttons to create a seamless experience.</p>
<p><strong>Caution</strong> - This feature is currently in beta version and only available to beta customers. To join the beta program, contact Adobe Customer Care.</p>
<img src="assets/do-not-localize/in-app.gif"/>
<p>For more information, refer to the <a href="../in-app/get-started-in-app.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Export Journey Optimizer Datasets to Cloud Storage Destinations (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now establish a live connection with cloud storage locations in order to export the content of your datasets. Available destinations are: Amazon S3 Cloud Storage, Azure Blob, Azure Data Lake Gen 2, Data Landing Zone, Google Cloud Storage, SFTP.</p>
<p><strong>Caution</strong> - This feature is currently in beta and available to all Adobe Journey Optimizer users. Please work with your Adobe representative on getting access to Destinations if you do not already have access.</p>
<img src="assets/do-not-localize/gif-destinations.gif"/>
<p>For more information, refer to the <a href="../data/export-datasets.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

<table>
<thead>
<tr>
<th><strong>Performance Measurement in campaigns</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now measure the performance of your campaigns across inbound and outbound through dedicated reports. Adobe Journey Optimizer reports can retrieve additional metrics to use in the <strong>Objective</strong> tab of your campaign reports. </p>
<img src="assets/do-not-localize/performance_report.gif"/>
<p>For more information, refer to the <a href="../privacy/data-hygiene.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

+++ Learn more about Performance Measurement

The **[!UICONTROL Objective]** tab of your Campaign report allows you to better fine-tune your deliveries' reports by targeting one specific metric. With this feature, you can effectively track and analyze your campaign's performance and make informed decisions to improve your results.

The **[!UICONTROL Objectives]** listed are linked to **[!UICONTROL Datasets]** that define a connection to a system in order to retrieve additional information. A list of pre-configured **[!UICONTROL Objectives]** is available, but you can also customize your report by adding new **[!UICONTROL Datasets]** and defining your own objectives. 

By selecting the desired Objectives, the **[!UICONTROL Performance overview]** and **[!UICONTROL Campaign objective]** widgets provide a comprehensive and insightful summary of your delivery performance, allowing you to closely monitor and evaluate the success of your campaign.

With the **[!UICONTROL Campaign objective]** widget, you can also choose to compare your primary objective against another performance metric.

Note that each widget can be resized and deleted as needed.
+++




<table>
<thead>
<tr>
<th><strong>Use Tags in your Journeys</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>As a Journey Optimizer practitioner, you can now organize your business objects using tags. Tags are a quick and easy way of classifying objects to improve search. Tags are currently only available for Journeys.</p>
</td>
</tr>
</tbody>
</table>

-->

### Improvements {#feb-2023-improvements}

**Journeys**

* The **Re-entrance wait period** field has been added to the journey properties. This field allows you to define the time to wait before allowing a profile to enter the journey again in unitary journeys (starting with an event or a segment qualification). This prevents journeys from being erroneously triggered multiple times for the same event. By default the field is set to 5 minutes. [Learn more](../building-journeys/journey-gs.md#entrance)

* Improvements have been made for **journey start and end dates**. If you have not specified a start date, it is now automatically added at publication time. For **Read segment** journeys, you can now add an end date. This allows profiles to exit automatically when the date is reached. [Learn more](../building-journeys/journey-gs.md#dates)

<!--

* The Journey canvas has been enhanced for a simpler and improved user experience. At the end of each path in the canvas, the empty placeholders have been removed. You can now simply add your activities by dragging them anywhere between nodes. [Learn more](../building-journeys/using-the-journey-designer.md)

* Timeout and error management has been improved in journeys. Timeout and error paths are now always added on the canvas. A new toolbar button is available to show/hide these paths. [Learn more](../building-journeys/journey-gs.md#timeout_and_error)

* A new type of system alert has been introduced. You can now get notified when a custom action fails. [Learn more](../reports/alerts.md)

* The Journey dashboard is now split in two tabs:
    * Use the **Overview** tab to access a new dashboard which displays key metrics related to your journeys.
    * Use the **Browse** tab to access list of all journeys.
-->


**Administration**

* **Allowed list** - You can now download the allowed list as a .csv file. [Learn more](../configuration/allow-list.md#download-allowed-list)

* **Email surface** - An additional check has been added to the email surface settings: if the MX record for the subdomain used in the **Reply to (email) address** or in the **BCC email address** is not properly configured, the email surface cannot be created anymore. You must have it configured or use another one. [Learn more](../email/email-settings.md#reply-to-email)

* **Email surface** - In the **URL tracking parameters** section of the email surface settings, the limit for each **Value** field has been updated from 255 characters to 5 KB for compatibility with Adobe Analytics tracking. [Learn more](../email/email-settings.md#url-tracking)

**Decision management**

* **Placements** - Additional parameters have been added in placements creation screen. They allow you to control whether an offer can be duplicated across multiple placements, and to specify if the offer's content and metadata should be included in the API response. [Learn more](../offers/offer-library/creating-placements.md)

* **URL personalization** - When adding URLs as content to your offers' representations, you can now personalize these URLs using the Expression Editor. [Learn more](../offers/offer-library/add-representations.md)

## January 2023 release notes{#jan-2023-release}

### New capabilities{#jan-2023-features}

<table>
<thead>
<tr>
<th><strong>Data Hygiene</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Platform provides a suite of data hygiene capabilities that allow you to manage your stored data through programmatic deletions of consumer records and datasets. This capability is now available for Adobe Journey Optimizer. </p>
<p>You can manage your data stores to ensure that information is used as expected, is updated when incorrect data needs fixing, and is deleted when organizational policies deem it necessary.</p>
<p><strong>Caution</strong> - Data Hygiene capabilities are currently only available for organizations that have purchased the <strong>Healthcare Shield</strong> and <strong>Privacy and Security Shield</strong> add-on offerings.</p><p>For more information, refer to the <a href="../privacy/data-hygiene.md">detailed documentation</a>.
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Email content templates</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create standalone content templates that can be leveraged across journeys and campaigns for quick reuse.</p> 
</p>
<img src="assets/do-not-localize/content-template.gif"/>
<p>Learn how to create, edit, and use content templates in <a href="https://experienceleague.adobe.com/docs/journey-optimizer-learn/tutorials/email-channel/content-templates.html">this video</a>. For more information, refer to the <a href="../email/content-templates.md">detailed documentation</a>.
</p>
</td>
</tr>
</tbody>
</table>

### Improvements {#jan-2023-improvements}

**Journeys**

* When adding a **Segment qualification** or **Read segment** in a journey, the namespace is now pre-filled, by default, with the last used namespace. Refer to the [Segment qualification](../building-journeys/segment-qualification-events.md#about-segment-qualification) and [Read segment](../building-journeys/read-segment.md#configuring-segment-trigger-activity) sections.

* In the journey canvas, a new button is available in the toolbar which allows you to download a screenshot of your journey. 

**Email Designer**

* You can now export the email content from the **Export HTML** menu. Exported files are available in an archive (.ZIP) file.

**Administration**

* A new subsection provides recommendations on building the **Reply to (email)** address and ensuring proper reply management. [Learn more](../email/email-settings.md#reply-to-email)

* When creating or editing **IP pools**, the associated PTR records are now displayed in the IP list and when hovering over the selected IP addresses. [Learn more](../configuration/ip-pools.md#create-ip-pool)

* After an IP pool has been selected in a channel surface, PTR record information is now visible when hovering over the IP addresses. [Learn more](../email/email-settings.md#subdomains-and-ip-pools)

* The user interface for editing [PTR records](../configuration/ptr-records.md#edit-ptr-record) and [execution fields](../configuration/primary-email-addresses.md) has been updated.

* The user interface for creating and editing subdomains has been improved. [Learn more](../configuration/delegate-subdomain.md)

* The suppression list **Recent uploads** screen has been updated. [Learn more](../configuration/manage-suppression-list.md#recent-uploads)

**Campaigns**

* A sample cURL request allowing API-triggered campaigns execution is now automatically generated and made available in the campaign screen. [Learn more](../campaigns/api-triggered-campaigns.md)


**Personalization**

* New helper functions are available: formatCurrency, charCodeAt, stringToDate, toString, formatNumber, and toHexString. Additionally, the toDateTimeOnly function now accepts string, date, long and int field types. [Learn more](../personalization/functions/functions.md)
