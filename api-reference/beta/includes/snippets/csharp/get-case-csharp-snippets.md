---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 223957223634b022f351f35317c14dbb87354aeb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @case = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Request()
    .GetAsync();

```