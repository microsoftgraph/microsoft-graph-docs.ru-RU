---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d871c2d327cfba4c29e9d6f5dc2bdef7c63140d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097855"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
options := &msgraphsdk.PersonInterestRequestBuilderPatchOptions{
    Body: requestBody,
}
personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Patch(options)


```