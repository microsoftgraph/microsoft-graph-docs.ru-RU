---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebc7ef3fa1601d14f3cd9bf94b71fb0bc2202ff3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Unsubmit(educationClass-id, educationAssignment-id, educationSubmission-id).Post(nil)


```