---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50fb9b3d16dc051faae8ce44b0ffdd1225cae5d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Print.Services["{printService-id}"].Endpoints
    .Request()
    .GetAsync();

```