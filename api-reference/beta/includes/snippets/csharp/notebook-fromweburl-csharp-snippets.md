---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae4dbfc9a13d045a10ac95d38a6d6ea0b8ed7734
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webUrl = "webUrl value";

await graphClient.Me.Onenote.Notebooks
    .GetNotebookFromWebUrl(webUrl)
    .Request()
    .PostAsync();

```