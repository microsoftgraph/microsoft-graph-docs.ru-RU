---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4bf9214aaf694fc1ebfb4a87423825ea72cab649
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = await graphClient.Domains["contoso.com"]
    .Request()
    .GetAsync();

```