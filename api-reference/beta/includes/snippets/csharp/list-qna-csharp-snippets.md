---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe07de79161bd22724e1c8ecd312294a3ec531e2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var qnas = await graphClient.Search.Qnas
    .Request()
    .GetAsync();

```