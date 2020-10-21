---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95061fa350a4a7497da2f1277b3642ace5cfaaf7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["{object-id}"]
    .Request()
    .GetAsync();

```