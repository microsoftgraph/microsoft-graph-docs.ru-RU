---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88f7638932661c2e78e2ffac5adb99987cde8e93ce4ab571d7537f9e3167aabf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57374245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"]
    .Request()
    .GetAsync();

```