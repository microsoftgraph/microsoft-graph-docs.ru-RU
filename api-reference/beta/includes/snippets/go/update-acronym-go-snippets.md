---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 373f02f2342d78cadaa5ccc407a34b9aa13e4b3a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAcronym()
description := "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
requestBody.SetDescription(&description)
options := &msgraphsdk.AcronymRequestBuilderPatchOptions{
    Body: requestBody,
}
acronymId := "acronym-id"
graphClient.Search().AcronymsById(&acronymId).Patch(options)


```