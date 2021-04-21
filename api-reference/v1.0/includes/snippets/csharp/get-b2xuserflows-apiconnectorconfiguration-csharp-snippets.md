---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d31fc0ffb320879d6eb590e4ff6ff15d21049f1
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .Expand("postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2xUserFlows.ApiConnectorConfiguration;

```