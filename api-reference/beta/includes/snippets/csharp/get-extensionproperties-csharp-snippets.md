---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37dd82c4e46be5917d4a7abe040bc617331d4427
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809850"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperties = await graphClient.Applications["{application-id}"].ExtensionProperties
    .Request()
    .GetAsync();

```