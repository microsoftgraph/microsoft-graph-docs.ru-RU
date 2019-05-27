---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 272ae40f8fb5373e7e02cd3b85a783cc2211fe67
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entityType = "Group";

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = "onBehalfOfUserId-value";

await graphClient.DirectoryObjects
    .ValidateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```