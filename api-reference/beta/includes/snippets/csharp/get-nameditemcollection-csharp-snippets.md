---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 826637c3f1d83ad7a820273cd97e13a02ee10c05
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Request()
    .GetAsync();

```