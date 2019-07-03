---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83d4bcb292d0a4020675fc40c82d8485a781a6a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions
    .Request()
    .GetAsync();

```