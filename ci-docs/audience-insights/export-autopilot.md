---
title: "Export Customer Insights data to Autopilot"
description: "Learn how to configure the connection to Autopilot."
ms.date: 12/08/2020
ms.reviewer: philk
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: m-hartmann
ms.author: mhart
manager: shellyha
---

# Connector for Autopilot (preview)

Export segments of unified customer profiles to Autopilot and use them for email marketing in Autopilot. 

## Prerequisites

-	You have an [Autopilot account](https://www.autopilothq.com/) and corresponding administrator credentials.
-	You have [configured segments](segments.md) in audience insights.
-	Unified customer profiles in the exported segments contain a field representing an email address.

## Connect to Autopilot

1. Go to **Admin** > **Export destinations**.

1. Under **Autopilot**, select **Set up**.

1. Give your export destination a recognizable name in the **Display name** field.

   :::image type="content" source="media/export-autopilot.PNG" alt-text="Configuration pane for Autopilot connection.":::

1. Enter your **Autopilot API key** [Autopilot API key](https://autopilot.docs.apiary.io/#).

1. Select **I agree** to confirm the **Data privacy and compliance**.

1. Select **Connect** to initialize the connection to Autopilot.

1. Select **Add yourself as export user** and provide your Customer Insights credentials.

1. Select **Next** to configure the export.

## Configure the connector

1. In the **Data matching** section, in the **Email** field, select the field in your unified customer profile that represents a customer's email address. Repeat the same steps for other optional fields such as **First name**, **Last name**.

1. Select the segments you want to export. We strongly **recommend to not export more than 100'000 customer profiles in total** to Autopilot. 

1. Select **Save**.

## Export the data

You can [export data on demand](export-destinations.md). The export will also run with every [scheduled refresh](system.md#schedule-tab).

## Known limitations

- You can export up to 100'000 profiles in total to Autopilot.
- Exporting to Autopilot is limited to segments.
- Exporting up to 100'000 profiles to Autopilot can take up to a few hours to complete. 
- The number of profiles that you can export to Autopilot is dependent and limited on your contract with Autopilot.

## Data privacy and compliance

When you enable Dynamics 365 Customer Insights to transmit data to Autopilot, you allow transfer of data outside of the compliance boundary for Dynamics 365 Customer Insights, including potentially sensitive data such as Personal Data. Microsoft will transfer such data at your instruction, but you are responsible for ensuring that Autopilot meet any privacy or security obligations you may have. For more information, see [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?linkid=396732).
Your Dynamics 365 Customer Insights Administrator can remove this export destination at any time to discontinue use of this functionality.