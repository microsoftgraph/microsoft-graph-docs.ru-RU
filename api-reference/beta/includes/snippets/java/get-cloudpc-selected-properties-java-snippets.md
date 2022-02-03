---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a66c12c9f2af6456714ad7d618a024746d432d1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPC cloudPC = graphClient.deviceManagement().virtualEndpoint().cloudPCs("40cee9d2-03fb-4066-8d35-dbdf2875c33f")
    .buildRequest()
    .select("id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult")
    .get();

```