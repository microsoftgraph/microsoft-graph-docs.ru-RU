---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cdd2b7c9f61824b3f20aff87d9b9827fc7e78eef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    IsLocked = true
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .UpdateAsync(conversationThread);

```