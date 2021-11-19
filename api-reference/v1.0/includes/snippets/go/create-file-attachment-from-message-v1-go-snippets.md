---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa0af75ea30775cc16058cc9d3ed14cedf00a04e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "smile"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "contentBytes": "R0lGODdhEAYEAA7",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Post(options)


```