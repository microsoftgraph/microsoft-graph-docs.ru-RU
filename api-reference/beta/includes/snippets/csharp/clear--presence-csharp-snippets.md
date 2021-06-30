---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 70083f97879b8cf1d2edd23c44fc4cc6f423dce9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

await graphClient.Users["{user-id}"].Presence
    .ClearPresence(sessionId)
    .Request()
    .PostAsync();

```