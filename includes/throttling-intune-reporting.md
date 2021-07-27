---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 1e0efd19d7ffec7e8f710187830582a6239402d2
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2021
ms.locfileid: "53579120"
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
