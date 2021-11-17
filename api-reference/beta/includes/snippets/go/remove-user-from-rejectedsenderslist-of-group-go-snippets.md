---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96616e503367060b86e2fd222b944dc158d9600b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981501"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RefRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/beta/users/%7Bid%7D",
}
options := &msgraphsdk.RefRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).RejectedSenders().$ref().Delete(options)


```