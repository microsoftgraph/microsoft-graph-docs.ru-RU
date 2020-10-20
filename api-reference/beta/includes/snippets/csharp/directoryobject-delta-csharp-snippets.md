---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd9e920f849acb8299eb59db38d24b66e59e555b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')")
    .GetAsync();

```