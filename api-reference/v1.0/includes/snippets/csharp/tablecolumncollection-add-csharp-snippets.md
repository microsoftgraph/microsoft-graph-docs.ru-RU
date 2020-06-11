---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 865803beffa9a7374cf65fffc465408da679c347
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684246"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

var values = JToken.Parse("[{}]");

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```