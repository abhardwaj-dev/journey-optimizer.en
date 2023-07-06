---
solution: Journey Optimizer
product: journey optimizer
title: Journey Optimizer guardrails and limitations
description: Learn more about Journey Optimizer guardrails
feature: Journeys
topic: Content Management
role: User
level: Intermediate
exl-id: 5d59f21c-f76e-45a9-a839-55816e39758a
---
# Guardrails and limitations {#limitations}

Entitlements, product limitations and performance guardrails are listed in [Adobe Journey Optimizer product description page](https://helpx.adobe.com/legal/product-descriptions/adobe-journey-optimizer.html){target="_blank"}.

You also need to be aware of [Guardrails for Real-time Customer Profile data before starting](https://experienceleague.adobe.com/docs/experience-platform/profile/guardrails.html){target="_blank"}.

You will find below additional guardrails and limitations when using [!DNL Adobe Journey Optimizer].

## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.

## Message guardrails {#message-guardrails}

* You cannot add attachments to an email with [!DNL Journey Optimizer].
* You cannot use the same sending domain to send out messages from [!DNL Adobe Journey Optimizer] and from another product, such as [!DNL Adobe Campaign] or [!DNL Adobe Marketo Engage] for example.


## Landing pages guardrails {#lp-guardrails}

* Only one **Form** component can be used in a single primary page.
* The **Form** component cannot be used in subpages.
* You cannot add a preheader to a landing page.
* You cannot select the **Code your own** option when designing a landing primary page.

## Journey guardrails {#journeys-guardrails}

### General journey guardrails {#journeys-guardrails-journeys}

* The number of activities in a journey is limited to 50. The number of activities is displayed on the upper left section of the journey canvas. This will help in readability, QA and troubleshooting. 

### General actions {#general-actions-g}

* There is no sending throttling.
* Three retries are systematically performed in case of an error. You cannot adjust the number of retries according to the error message received.
* The built-in **Reaction** event allows you to react to out-of-the-box actions. Learn more in [this page](../building-journeys/reaction-events.md). If you want to react to a message sent via a custom action, you need to configure a dedicated event.
* You cannot place two actions in parallel, you must add them one after the other.
* A profile cannot be present multiple times in the same journey, at the same time. If re-entrance is enabled, a profile can reenter a journey, but cannot do it until it fully exits the previous instance of the journey. [Read more](../building-journeys/end-journey.md)

### Journey versions {#journey-versions-g}

* A journey starting with an event activity in v1 cannot start with something else than an event in further versions. You cannot start a journey with a **Segment Qualification** event. 
* A journey starting with a **Segment Qualification** activity in v1 must always start with a **Segment Qualification** in further versions. 
* The segment and namespace chosen in **Segment Qualification** (first node) cannot be changed in new versions.
* The re-entrance rule must be the same in all journey versions.
* A journey starting with a **Read Segment** cannot start with another event in next versions.
* You cannot create a new version of a read segment journey with incremental read. You need to duplicate the journey.

### Custom actions {#custom-actions-g}

* The custom action URL does not support dynamic parameters.
* Only POST and PUT call methods are supported
* The name of the query parameter or header must not start with "." or "$"
* IP addresses are not allowed
* Internal Adobe addresses (`.adobe.*`) are not allowed in URLs and APIs.
* Built-in custom actions cannot be removed.

### Events {#events-g}

* For system-generated events, streaming data used to initiate a customer journey must be configured within Journey Optimizer first to get a unique orchestration ID. This orchestration ID must be appended to the streaming payload coming into Adobe Experience Platform. This limitation does not apply to rule-based events.
* Business events cannot be used in conjunction with unitary events or segment qualification activities.
* Unitary journeys (starting with an event or a segment qualification) include a guardrail that prevents journeys from being erroneously triggered multiple times for the same event. Profile re-entrance is temporally blocked by default for 5 minutes. For instance, if an event triggers a journey at 12:01 for a specific profile and another one arrives at 12:03 (whether it is the same event or a different one triggering the same journey) that journey will not start again for this profile.
* Journey Optimizer requires events to be streamed to Data Collection Core Service (DCCS) to be able to trigger a journey. Events ingested in batch or events from internal Journey Optimizer datasets (Message Feedback, Email Tracking, etc.) cannot be used to trigger a journey. For use cases where you cannot get streamed events, please build a segment based on those events and use the **Read Segment** activity instead. Segment qualification can technically be used, but can cause downstream challenges based on the actions used.

### Data sources {#data-sources-g}

* External data sources can be leveraged within a customer journey to lookup external data in real time. These sources must be usable via REST API, support JSON and be able to handle the volume of requests.
* Internal Adobe addresses (`.adobe.*`) are not allowed in URLs and APIs.

### Journeys and profile creation {#journeys-limitation-profile-creation}
 
There is a delay associated to API based profile creation/update in Adobe Experience Platform. The Service Level Target (SLT) in terms of latency is < 1 min from ingestion to Unified Profile for 95th percentile of requests, at a volume of 20K Requests per second (RPS).

If a journey is triggered simultaneously to a profile creation and immediately checks/retrieves information from Profile Service, it might not work properly.

You can choose from one of these two solutions:

* Add a wait activity after the first event, to give Adobe Experience Platform the time it needs to perform the ingestion to Profile Service.

* Set up a journey that does not immediately leverage the profile. For example, if the journey is designed to confirm an account creation, the experience event could contain information needed to send the first confirmation message (first name, last name, email address, etc.). 

### Read segment {#read-segment-g}

* Streamed segments are always up-to-date but batch segments will not be calculated at retrieval time. They are only evaluated every day at the daily batch evaluation time.
* For journeys using a Read Segment activity, there is a maximum number of journeys that can start at the exact same time. Retries will be performed by the system but please avoid having more than five journeys (with Read Segment, scheduled or starting "as soon as possible") starting at the exact same time by spreading them over time, for example 5 to 10 minutes apart.

### Expression editor {#expression-editor}

* Experience event field groups can not be used in journeys starting with a Read segment, a Segment qualification or a business event activity. You need to create a new segment and use an "in segment" condition in the journey.


