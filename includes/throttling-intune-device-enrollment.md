---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: c2a090958916e0535a0410929c4f8bf366bc484bc5692a4235725f6fe999d9e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196772"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-device-enrollment-service-limits"></a>Ограничения службы регистрации устройств Intune

| Тип запроса | Ограничение на клиента для всех приложений | Ограничение на приложение по клиенту |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELETE, PATCH | 200 запросов за 20 секунд | 100 запросов за 20 секунд |
| Любой | 2000 запросов за 20 секунд | 1000 запросов за 20 секунд |

Указанные выше ограничения действуют для следующих ресурсов:  
complianceManagementPartner, deviceAppManagement, deviceCategory, deviceComanagementAuthorityConfiguration, deviceEnrollmentConfiguration, deviceEnrollmentLimitConfiguration, deviceEnrollmentPlatformRestrictionsConfiguration, deviceEnrollmentWindowsHelloForBusinessConfiguration, deviceManagementExchangeConnector, deviceManagementExchangeOnPremisesPolicy, deviceManagementPartner, enrollmentConfigurationAssignment, mobileThreatDefenseConnector, onPremisesConditionalAccessSettings, sideLoadingKey, vppToken, windows10EnrollmentCompletionPageConfiguration.
