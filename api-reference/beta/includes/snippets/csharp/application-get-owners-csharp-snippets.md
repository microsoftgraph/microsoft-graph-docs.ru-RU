---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88659fa1c4a77c5a4e72fb63cb0f6318c68cdf38
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Applications["{application-id}"].Owners
    .Request()
    .GetAsync();

```