---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: beb55d607bc4d15780afb2c82f8c920ded48dbf2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```