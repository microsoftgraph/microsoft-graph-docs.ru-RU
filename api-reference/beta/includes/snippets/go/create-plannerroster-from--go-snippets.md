---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da38888aa9e13321aca2f9115f3c59b80e94d68c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097958"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerRoster()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.plannerRoster",
}
options := &msgraphsdk.RostersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Rosters().Post(options)


```