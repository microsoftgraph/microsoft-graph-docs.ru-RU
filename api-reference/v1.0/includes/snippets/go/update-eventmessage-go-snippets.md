---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a22242472f37d14cd4e307bd3513d76ce5718da8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
isRead := true
requestBody.SetIsRead(&isRead)
options := &msgraphsdk.MessageRequestBuilderPatchOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(options)


```