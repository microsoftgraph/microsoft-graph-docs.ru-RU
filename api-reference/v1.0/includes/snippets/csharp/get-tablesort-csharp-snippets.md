---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b56a1f79421db2941bed08568f70fddba3ebb220a302bec8047b8a4bd7655ec9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57325017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableSort = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Request()
    .GetAsync();

```