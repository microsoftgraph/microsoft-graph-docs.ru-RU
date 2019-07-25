---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ea35d4442b48be4ef2502fcbecf5065a395032db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709033"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var all = true;

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .CancelMediaProcessing(all,clientContext)
    .Request()
    .PostAsync();

```