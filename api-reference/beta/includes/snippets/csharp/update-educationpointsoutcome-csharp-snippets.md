---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 76fef53bc20acb05f6611de0c6afcc4fa3bf7349
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationPointsOutcome
{
    Points = new EducationAssignmentPointsGrade
    {
        Points = 85f
    }
};

await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```