---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0cfb221772fd5ce974ee25901e2520f2c55c1975
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35515303"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.SectionGroups["{id}"].Sections
    .Request()
    .GetAsync();

```