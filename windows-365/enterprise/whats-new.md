---
# required metadata
title: What's new in Windows 365 Enterprise
titleSuffix:
description: Find out what's new in Windows 365 Enterprise
keywords:
author: ErikjeMS  
ms.author: erikje
manager: dougeby
ms.date: 10/05/2021
ms.topic: reference
ms.service: cloudpc
ms.subservice:
ms.localizationpriority: high
ms.technology:
ms.assetid: 

# optional metadata

#ROBOTS:
#audience:

ms.reviewer: traceyadams
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure; get-started
ms.collection: M365-identity-device-management
---

# What's new in Windows 365 Enterprise

Learn what new features are available in Windows 365 Enterprise.

> [!Note]
> Each monthly update may take up to a week to rollout to all customers.

<!-- Common categories:  
### App management
### Device configuration
### Device provisioning
### Device management
### Device security
### Intune apps
### Monitor and troubleshoot
### Role-based access control
### Scripts
-->

<!-- ########################## -->
## Week of October 11, 2021 (Service release 2109)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Device management

#### Resize support for preview and trial licenses<!--36228235-->

If you have a combination of paid and free trial licenses, the Resize remote action will use your paid licenses first. When those run out, it will use your trial licenses. For more information, see [Resize a Cloud PC](resize-cloud-pc.md).

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Device provisioning

#### Health check improvement<!--36461502-->

The **DNS can resolve Active Directory domain** health check has been improved. A new step has been added to look for the following Azure Active Directory DNS record. If it can’t be found, the check fails.

_ldap._tcp.yourDomain.com -type SRV

<!-- ########################## -->
## Week of October 4, 2021
<!-- vvvvvvvvvvvvvvvvvvvvvv -->

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Device management

#### Support for Windows 11<!--35091970 -->

Windows 365 Enterprise now supports Windows 11 as a Cloud PC operating system.

Windows 11 Cloud PCs require Generation 2 (Gen2) virtual machines. For information about converting existing Generation 1 custom device images to Gen2, see [Convert an existing custom device image to a generation 2 virtual machine](device-images-convert-generation-2.md).

## Week of September 13, 2021
<!-- vvvvvvvvvvvvvvvvvvvvvv -->

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Device management

#### New PowerShell script for installing languages on custom device images<!--35726116-->

The [Windows365LanguagesInstaller PowerShell script]( https://www.powershellgallery.com/packages/Windows365LanguagesInstaller) can install 38 additional languages on your custom device images. For more information, see [Provide a localized Windows experience](provide-localized-windows-experience.md#add-languages-to-windows-using-a-script-and-capture-the-image).

<!-- ########################## -->
## Week of September 6, 2021 (Service release 2108)

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Device management

#### End grace period option<!--34841603-->

Certain conditions put a Cloud PC into a seven-day grace period. At the end of this time the Cloud PC will be deprovisioned and user will lose access.

You can now immediately end the grace period for individual Cloud PCs. By ending the grace period manually, you won’t have to wait the full seven days to remove user access from the Cloud PC.

For more information on grace periods, see [End grace period](end-grace-period.md).

<!-- ########################## -->
## Week of August 30, 2021

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
### Monitor and troubleshoot

#### Resource performance report in Endpoint Analytics<!-- 32978343 -->

Endpoint analytics has a new report named **Resource performance**. The **Resource performance report** includes metrics for CPU and RAM performance on Cloud PCs. For more information, see [Resource performance report](report-resource-performance.md).

#### Remoting connection report in Endpoint Analytics<!-- 33039368 -->

Endpoint analytics has a new report named **Remoting connection report**. This report includes the following metrics:

- **Cloud PC Sign in time (sec)** provides the total time users take to connect to the cloud PC.
- **Round Trip Time (ms)** provides insights on the speed and reliability of network connections from the user location.

For more information, see [Remoting connection report](report-remoting-connection.md).

<!-- ########################## -->
## Week of August 2, 2021

<!-- vvvvvvvvvvvvvvvvvvvvvv -->
<!--### Feature area alpha-->

### Windows 365 now generally available<!--10393594 -->

Windows 365 is a new service from Microsoft that automatically creates Cloud PCs for your end users. Cloud PCs are a new hybrid personal computing category that use both the power of the cloud and the accessing device to provide a full and personalized Windows virtual machine. Admins can use Microsoft Endpoint Manager to define the configurations and applications that are provisioned for each user’s Cloud PC. End users can access their Cloud PC from any device and any location. Windows 365 stores the end user’s Cloud PC and data in the cloud, not on the device, providing a secure experience.

For more information about Windows 365, see [Windows 365](https://www.microsoft.com/windows-365?rtc=1).

<!-- ########################## -->
## Next steps

For details about Windows 365 licensing, see [Windows 365 pricing](https://www.microsoft.com/windows-365/enterprise/compare-plans-pricing).
