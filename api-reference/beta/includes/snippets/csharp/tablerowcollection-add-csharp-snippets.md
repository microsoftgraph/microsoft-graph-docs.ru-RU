---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97c6f7b10f5a176b63a04e6fc099c38d4d0b3ad1
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = null;

var values = new List<Json>()
{
    new List<Json>()
{
    1,
    2,
    3
},
    new List<Json>()
{
    4,
    5,
    6
}
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```