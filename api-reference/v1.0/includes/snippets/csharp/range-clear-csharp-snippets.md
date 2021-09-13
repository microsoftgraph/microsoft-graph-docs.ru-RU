---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db22902ae39a9c6c2c8a02b74eac79eca9c1fb0f54014a7fcd4bdd08c8450ff5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applyTo = "applyTo-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Clear(applyTo)
    .Request()
    .PostAsync();

```