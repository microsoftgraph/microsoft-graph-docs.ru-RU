---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e9ccedb2d066c7c98762c2b653db1292550daab6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```