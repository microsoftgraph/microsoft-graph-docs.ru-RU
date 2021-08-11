---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: b6ad2566d019a6d9fb8ecb90f83b594de4ea6eb2ebc18e58cfd896732a6e1520
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196776"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-endpoint-protection-service-limits"></a>Ограничения службы защиты конечных точек Intune

| Тип запроса | Ограничение на клиента для всех приложений | Ограничение на приложение по клиенту |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELETE, PATCH | 200 запросов за 20 секунд | 100 запросов за 20 секунд |
| Любой | 2000 запросов за 20 секунд | 1000 запросов за 20 секунд |

Указанные выше ограничения действуют для следующих ресурсов:  
deviceManagementDerivedCredentialSettings, deviceManagementResourceAccessProfileAssignment, deviceManagementResourceAccessProfileBase, windows10XCertificateProfile, windows10XSCEPCertificateProfile, windows10XTrustedRootCertificate, windows10XVpnConfiguration, windows10XWifiConfiguration.
