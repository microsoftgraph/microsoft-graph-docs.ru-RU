---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa8bc94e1c9e999ed1581507d9a80b94f522e079
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Users["{educationUser-id}"].Assignments
    .Request()
    .GetAsync();

```