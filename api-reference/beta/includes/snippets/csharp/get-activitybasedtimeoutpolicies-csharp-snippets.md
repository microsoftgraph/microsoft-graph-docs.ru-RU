---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 827eed4ed517a7fd3b0e730650b7d7e46de74e8d
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policy = await graphClient.Policies["activityBasedTimeoutPolicies"]
    .Request()
    .GetAsync();

```