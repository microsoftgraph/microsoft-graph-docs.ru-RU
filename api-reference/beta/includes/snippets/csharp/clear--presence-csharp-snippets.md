---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1342d628c083299a4a119986a6e9e3cea8167eb33517296f282b8a89589bbe52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57209894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

await graphClient.Users["{user-id}"].Presence
    .ClearPresence(sessionId)
    .Request()
    .PostAsync();

```