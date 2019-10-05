---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca9f78d75db63117827853779914a67f8f4c115c
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

var values = new List<Json>()
{
    new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```