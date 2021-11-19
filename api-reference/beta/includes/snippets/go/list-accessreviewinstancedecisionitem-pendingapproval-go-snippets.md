---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae3d01632fee12e643a078a438a536d5b004c965
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DecisionsRequestBuilderGetQueryParameters{
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.DecisionsRequestBuilderGetOptions{
    Q: requestParameters,
}
accessReviewInstanceId := "accessReviewInstance-id"
result, err := graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).Decisions().Get(options)


```