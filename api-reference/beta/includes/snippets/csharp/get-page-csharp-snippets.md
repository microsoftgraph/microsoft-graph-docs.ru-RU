---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d93fa7cb5282aa6e0ad2ae4b4fb9cf925828b375
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{page-id}"]
    .Request()
    .GetAsync();

```