---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 56bf74e1abd3a3231fd16e827cc200f031173ff3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095600"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Expand: "extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```