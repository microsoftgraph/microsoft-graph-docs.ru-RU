---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 968d40861864abf5b527210f8cfab6b0766c7ae6
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "66041036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChecklistItem()
displayName := "Final sign-off from the team"
requestBody.SetDisplayName(&displayName)
todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).ChecklistItems().Post(requestBody)


```