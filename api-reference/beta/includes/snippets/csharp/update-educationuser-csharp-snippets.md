---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c2ef9fb22dbd6ba3accd317714066f9ae2f8e38
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    DisplayName = "Rogelio Cazares",
    GivenName = "Rogelio",
    MiddleName = "Fernando",
    Surname = "Cazares"
};

await graphClient.Education.Users["13020"]
    .Request()
    .UpdateAsync(educationUser);

```