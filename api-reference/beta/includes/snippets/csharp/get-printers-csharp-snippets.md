---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1efb91f1ccc180417c1912315a178695bbb0446
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "42948319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printers = await graphClient.Print.Printers
    .Request()
    .GetAsync();

```