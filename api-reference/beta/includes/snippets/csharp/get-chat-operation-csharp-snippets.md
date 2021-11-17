---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d4c7db339eb0e8048bf35d2f83a1c80e5f7acdab135e2dd247d8ccff28ec6228
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAsyncOperation = await graphClient.Chats["{chat-id}"].Operations["{teamsAsyncOperation-id}"]
    .Request()
    .GetAsync();

```