---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14d1354612dcff9cc0a857e6c2ab134262082dcc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440611"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("60b94f83-3e22-430e-a69d-440f65b922d6")
    .buildRequest()
    .select("id,description,displayName,domainJoinConfiguration,imageDisplayName,imageId,imageType,onPremisesConnectionId,windowsSettings,managedBy,cloudPcGroupDisplayName,gracePeriodInHours,localAdminEnabled,alternateResourceUrl")
    .get();

```