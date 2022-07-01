---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 168f94d40daeee2aa674e122ef40f73ca233e614
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "66604506"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicy crossTenantAccessPolicy = new CrossTenantAccessPolicy();
LinkedList<String> allowedCloudEndpointsList = new LinkedList<String>();
allowedCloudEndpointsList.add("microsoftonline.us");
allowedCloudEndpointsList.add("partner.microsoftonline.cn");
crossTenantAccessPolicy.allowedCloudEndpoints = allowedCloudEndpointsList;

graphClient.policies().crossTenantAccessPolicy()
    .buildRequest()
    .patch(crossTenantAccessPolicy);

```