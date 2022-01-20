---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aeb2532d89a2822f080e687e7a054b56e6ae7221
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124221"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
destinationTaskListId := "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG"
requestBody.SetDestinationTaskListId(&destinationTaskListId)
options := &msgraphsdk.MoveRequestBuilderPostOptions{
    Body: requestBody,
}
baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).Move().Post(options)


```