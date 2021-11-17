---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ef1fc894bb3989abb0596955fc9ecac518a696b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020334"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSubjectRightsRequest()
internalDueDateTime, err := time.Parse(time.RFC3339, "2021-08-30T00:00:00Z")
requestBody.SetInternalDueDateTime(&internalDueDateTime)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.subjectRightsRequest",
}
options := &msgraphsdk.SubjectRightsRequestRequestBuilderPatchOptions{
    Body: requestBody,
}
subjectRightsRequestId := "subjectRightsRequest-id"
graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Patch(options)


```