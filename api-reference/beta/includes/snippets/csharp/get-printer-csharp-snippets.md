---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 447bc1f389634588c8e7dd2f7c3a414b2d108dc4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .GetAsync();

```