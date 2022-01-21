---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 412d8a7d45225a779a666364deaaaa3aa5170f51
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationCategory = new EducationCategory
{
    DisplayName = "Quizzes"
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Request()
    .AddAsync(educationCategory);

```