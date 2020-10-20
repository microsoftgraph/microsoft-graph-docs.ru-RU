---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ad5ecfad41d37b64a55cbb2eb2438a00877d2a5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{id}"]
    .Request()
    .GetAsync();

```