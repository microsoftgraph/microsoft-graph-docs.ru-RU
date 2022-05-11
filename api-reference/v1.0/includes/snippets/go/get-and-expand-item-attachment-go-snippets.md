---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58cbdab96475ea292e9c32fa6b0957a58927d04c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttachmentRequestBuilderGetQueryParameters{
    Expand: "microsoft.graph.itemattachment/item",
}
options := &msgraphsdk.AttachmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
messageId := "message-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().MessagesById(&messageId).AttachmentsById(&attachmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```