---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68b248900b57b6164937f3b569fa5d2bb0c62470
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents
    .Request()
    .GetAsync();

```