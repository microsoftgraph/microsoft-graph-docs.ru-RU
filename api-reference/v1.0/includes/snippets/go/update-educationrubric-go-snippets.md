---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91eadfde4eee103e02682b08c25f992cb9693606
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095713"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric after display name patch"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.EducationRubricRequestBuilderPatchOptions{
    Body: requestBody,
}
educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Patch(options)


```