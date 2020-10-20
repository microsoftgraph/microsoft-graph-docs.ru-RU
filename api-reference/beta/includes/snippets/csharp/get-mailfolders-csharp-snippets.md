---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 988379b0f1f73bbff16c66dc5df4999258d89eb0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolders = await graphClient.Me.MailFolders
    .Request()
    .GetAsync();

```