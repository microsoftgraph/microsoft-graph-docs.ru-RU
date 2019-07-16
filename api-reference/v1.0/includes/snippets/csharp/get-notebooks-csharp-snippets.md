---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b2936b66a608d86810f1ee940254f135684a0b2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebooks = await graphClient.Me.Onenote.Notebooks
    .Request()
    .GetAsync();

```