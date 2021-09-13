---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a4d23a64e2c4ce37754a31ab830f4d782268b596c5755f934a69e10b9e788e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test5";

var reference = JsonDocument.Parse(@"""=Sheet1!$F$15:$N$27""");

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Add(name,reference,comment)
    .Request()
    .PostAsync();

```