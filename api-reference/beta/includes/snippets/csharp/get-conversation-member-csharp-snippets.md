---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 72be751d7f6712ade1a8366e856aa1382d3ad8df
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Chats["19:cf66807577b149cca1b7af0c32eec122@thread.v2"].Members["141c574c-dd90-4131-b173-baf4bb0e894e"]
    .Request()
    .GetAsync();

```