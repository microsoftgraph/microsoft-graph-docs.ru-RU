---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c04e13f3beae0771ae68880206e3dba0d1ffb56b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522584"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICloudPcProvisioningPolicyCollectionPage provisioningPolicies = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies()
    .buildRequest()
    .get();

```