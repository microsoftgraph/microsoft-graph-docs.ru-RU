---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9fab5cf52a5034dadf18370ad1d9a28e26676358
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupRequestBuilderGetQueryParameters{
    Select: "allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount",
}
options := &msgraphsdk.GroupRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```