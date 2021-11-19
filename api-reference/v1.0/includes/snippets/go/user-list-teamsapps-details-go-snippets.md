---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 808d44d30d2de167599abc5b113a417befea21b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.InstalledAppsRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.InstalledAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledApps().Get(options)


```