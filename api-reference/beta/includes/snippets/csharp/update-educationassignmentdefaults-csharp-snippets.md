---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81caee5ffdd47652bd9ec2a084be48668ad69b222c99ca3da18c4de5f374cceb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = new EducationAssignmentDefaults
{
    AddedStudentAction = EducationAddedStudentAction.AssignIfOpen,
    AddToCalendarAction = EducationAddToCalendarOptions.StudentsAndTeamOwners,
    NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')"
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentDefaults
    .Request()
    .UpdateAsync(educationAssignmentDefaults);

```