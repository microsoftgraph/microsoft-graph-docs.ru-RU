---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d078030ec9fc5f62838a4f88f51d894b1a7e14b4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskTriggers = await graphClient.Print.Printers["{id}"].TaskTriggers
    .Request()
    .GetAsync();

```