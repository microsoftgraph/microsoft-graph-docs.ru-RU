---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba7a6123addb0f072395a7b4b17e66f6866e5dac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DisplayName = "Week 1 reading assignment",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapters 1 through 3"
    },
    DueDateTime = DateTimeOffset.Parse("2014-02-01T00:00:00Z")
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .UpdateAsync(educationAssignment);

```