---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: beb55d607bc4d15780afb2c82f8c920ded48dbf2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```