---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37e1e5df790fea4237c7ef08fd090e8c8787dc7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950009"
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