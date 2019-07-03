---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 08df1a545a9cd144fa4f2df700d36ecae23c2401
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Groups["{id}"].Endpoints
    .Request()
    .GetAsync();

```