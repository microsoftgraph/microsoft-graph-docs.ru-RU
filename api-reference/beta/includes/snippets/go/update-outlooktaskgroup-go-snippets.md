---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ea1d7a933f75f816887927b17c2c58215743ace
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099154"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskGroup()
name := "Personal Tasks"
requestBody.SetName(&name)
options := &msgraphsdk.OutlookTaskGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookTaskGroupId := "outlookTaskGroup-id"
graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).Patch(options)


```