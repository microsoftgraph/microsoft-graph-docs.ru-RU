---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d90d01ea668ca34f735a6d8ff1576cc709722ae4
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].Jobs["{id}"].Documents["{id}"]
    .UploadData()
    .Request()
    .Header("Range","bytes=0-72796")
    .PostAsync();

```