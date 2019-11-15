---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35ef8b014af45c52fbb4f30d3989c1a8b97fb347
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordCredential = new PasswordCredential
{
    DisplayName = "Password friendly name"
};

await graphClient.Applications["{id}"]
    .AddPassword(passwordCredential)
    .Request()
    .PostAsync();

```