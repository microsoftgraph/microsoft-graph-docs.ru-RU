---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1a405599bc1c606af2e2e2e655824d6fc5b73ead
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["8b081ef6-4792-4def-b2c9-c363a1bf41d5"].Chats
    .Request()
    .Filter("members/any(o: o/displayname eq 'Peter Parker')")
    .Expand("members")
    .GetAsync();

```