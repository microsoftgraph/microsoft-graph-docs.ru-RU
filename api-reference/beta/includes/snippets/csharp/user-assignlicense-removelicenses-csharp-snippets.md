---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6925c490fee4462ca9f77dd8757c922803f5f1d9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63340017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
};

var removeLicenses = new List<Guid>()
{
    Guid.Parse("f30db892-07e9-47e9-837c-80727f46fd3d"),
    Guid.Parse("84a661c4-e949-4bd2-a560-ed7766fcaf2b")
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```