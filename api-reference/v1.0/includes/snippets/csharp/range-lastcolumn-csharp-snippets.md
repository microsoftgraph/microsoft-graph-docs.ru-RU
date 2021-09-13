---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4bb3febbf5075a696acd88e5cde05fc665006aaa66045fc10d8491cca074e1aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57369007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .LastColumn()
    .Request()
    .GetAsync();

```