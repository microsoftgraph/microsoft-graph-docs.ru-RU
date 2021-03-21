---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ddaa51f960fd65909793ac85e1b609212ff2830
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.Print.Services
    .Request()
    .GetAsync();

```