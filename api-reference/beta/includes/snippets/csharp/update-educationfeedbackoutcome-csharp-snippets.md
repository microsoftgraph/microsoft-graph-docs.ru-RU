---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac7a3c555c75650fd54cd86d7f71e0273abc14ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807972"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationFeedbackOutcome
{
    Feedback = new EducationFeedback
    {
        Text = new EducationItemBody
        {
            Content = "This is feedback for the assignment as a whole.",
            ContentType = BodyType.Text
        }
    }
};

await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```