---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b576c0e09094c2197428c6d34d8632a7b757f92
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acronym = await graphClient.Search.Acronyms["{search.acronym-id}"]
    .Request()
    .GetAsync();

```