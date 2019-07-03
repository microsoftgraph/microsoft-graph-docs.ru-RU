---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d93fa7cb5282aa6e0ad2ae4b4fb9cf925828b375
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{page-id}"]
    .Request()
    .GetAsync();

```