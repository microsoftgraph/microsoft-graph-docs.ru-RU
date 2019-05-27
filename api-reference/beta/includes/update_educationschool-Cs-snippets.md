---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef7b372b4785b626b41c4ce11757c47426344eba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468748"
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