---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2820245e133b1b1a7f442ff52b84678825eb03fd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102286"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnotation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.PersonAnnotationRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
personAnnotationId := "personAnnotation-id"
graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Patch(options)


```