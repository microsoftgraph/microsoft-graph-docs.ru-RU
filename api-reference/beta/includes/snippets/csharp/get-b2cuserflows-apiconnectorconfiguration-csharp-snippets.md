---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99c7e9c94620f030605b4e33dba6c980a95506ee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .Expand("postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2cUserFlows.ApiConnectorConfiguration;

```