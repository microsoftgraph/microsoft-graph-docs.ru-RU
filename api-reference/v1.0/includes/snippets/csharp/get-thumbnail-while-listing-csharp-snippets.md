---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f46eb56c60abda9a798c4d21f61cdc361c4ed90d5dd8116786cbdc750311d342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394989"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{driveItem-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```