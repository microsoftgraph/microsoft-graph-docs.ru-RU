---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b2936b66a608d86810f1ee940254f135684a0b2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebooks = await graphClient.Me.Onenote.Notebooks
    .Request()
    .GetAsync();

```