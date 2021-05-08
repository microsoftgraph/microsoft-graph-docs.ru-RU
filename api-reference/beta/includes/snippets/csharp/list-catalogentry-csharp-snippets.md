---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1110c96cfb7592b7baf8b25eaffef36e5fcda0d9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entries = await graphClient.Admin.Windows.Updates.Catalog.Entries
    .Request()
    .GetAsync();

```