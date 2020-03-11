---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f92b275432b719f621d3d988213da23b8b7e5108
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Policies.TokenLifetimePolicies
    .Request()
    .GetAsync();

```