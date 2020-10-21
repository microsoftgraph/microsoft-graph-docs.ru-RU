---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de0e347856abdac5711bdf4d63388b1d003a4d8c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Sites["{siteId}"].Drives
    .Request()
    .GetAsync();

```