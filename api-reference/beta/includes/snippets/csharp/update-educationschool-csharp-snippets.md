---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef7b372b4785b626b41c4ce11757c47426344eba
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["10002"]
    .Request()
    .UpdateAsync(educationSchool);

```