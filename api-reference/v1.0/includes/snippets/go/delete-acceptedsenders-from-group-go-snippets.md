---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8d7e59c9e212d67c4005d3f5ef755a1644042b90
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RefRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D",
}
options := &msgraphsdk.RefRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).AcceptedSenders().$ref().Delete(options)


```