---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77460a343832a5f3ab248a4b55a26e20f5903d7c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997820"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Cooking"
requestBody.SetName(&name)
options := &msgraphsdk.TaskFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
outlookTaskGroupId := "outlookTaskGroup-id"
result, err := graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).TaskFolders().Post(options)


```