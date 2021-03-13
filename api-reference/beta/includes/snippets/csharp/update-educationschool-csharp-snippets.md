---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af073c534a4bf075e317ec5798eb5eed4b94f6c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam Arts High School",
    Description = "Magnate school for the arts. Los Angeles School District"
};

await graphClient.Education.Schools["{educationSchool-id}"]
    .Request()
    .UpdateAsync(educationSchool);

```