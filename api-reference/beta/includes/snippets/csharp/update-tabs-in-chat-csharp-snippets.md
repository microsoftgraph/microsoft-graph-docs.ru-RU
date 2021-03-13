---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37e1e5df790fea4237c7ef08fd090e8c8787dc7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = new TeamsTab
{
    DisplayName = "My Contoso Tab - updated again"
};

await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .UpdateAsync(teamsTab);

```