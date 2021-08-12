---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 17b5355ba3a51308822c5870d5ca0beafd5bf4ae69abc7914768f0cd1757b9c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196803"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-reporting-service-limits"></a>Ограничения службы отчетов Intune

| Тип запроса | Ограничение на клиента для всех приложений | Ограничение на приложение по клиенту |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELETE, PATCH | 200 запросов за 20 секунд | 100 запросов за 20 секунд |
| Любой | 2000 запросов за 20 секунд | 1000 запросов за 20 секунд |

Указанные выше ограничения действуют для следующих ресурсов:  
applicationSignInDetailedSummary, applicationSignInSummary, auditLogRoot, authenticationMethodsRoot, azureADFeatureUsage, azureADLicenseUsage, azureADUserFeatureUsage, credentialUsageSummary, credentialUserRegistrationCount, credentialUserRegistrationDetails, directoryAudit, provisioningObjectSummary, recommendation, recommendationResource, relyingPartyDetailedSummary, restrictedSignIn, signIn, userCredentialUsageDetails.
