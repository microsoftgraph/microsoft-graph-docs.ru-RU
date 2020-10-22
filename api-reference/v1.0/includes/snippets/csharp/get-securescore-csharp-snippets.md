---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 460bc93c7e2ebcde55a74533e6849be06b62958d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScore = await graphClient.Security.SecureScores["{id}"]
    .Request()
    .GetAsync();

```