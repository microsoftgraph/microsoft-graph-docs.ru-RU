---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73eca399dca6a6b70a067287bfb1336e9bb6821b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719708"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.GroupRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).TransitiveMembers().Group(group-id).GetWithRequestConfigurationAndResponseHandler(options, nil)


```