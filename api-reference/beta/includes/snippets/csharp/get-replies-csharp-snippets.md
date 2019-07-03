---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8525273f3ec881b6b1e3003819ed5894c9bd589c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Chats["{id}"].Messages["{id}"].Replies
    .Request()
    .GetAsync();

```