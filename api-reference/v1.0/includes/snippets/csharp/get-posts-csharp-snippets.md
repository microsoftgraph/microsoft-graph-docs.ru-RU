---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9f8964b5fcb0f1d2b93591cdff6f68400a0199ed
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["{id}"].Threads["{id}"].Posts
    .Request()
    .GetAsync();

```