---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c2f55681c11c1f854715227faecaf95a80b9210a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478904"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "Seattle District Technical Schools",
    Description = "Seattle district technical schools administration",
    Visibility = "true"
};

await graphClient.AdministrativeUnits
    .Request()
    .AddAsync(administrativeUnit);

```