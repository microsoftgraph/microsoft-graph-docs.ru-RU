---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 74af7cd688d894c294fcfcbaac4998d49377ba2c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435202"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = "The contents of the file goes here."

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .PutAsync(Stream);

```