---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6edad942149945e87103d8233eae83464267a6ec
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977260"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Travel items"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ListsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Todo().Lists().Post(options)


```