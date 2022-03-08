---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 74a30152fdba72c19281812c4023f7b81d263f7c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acronyms = await graphClient.Search.Acronyms
    .Request()
    .GetAsync();

```