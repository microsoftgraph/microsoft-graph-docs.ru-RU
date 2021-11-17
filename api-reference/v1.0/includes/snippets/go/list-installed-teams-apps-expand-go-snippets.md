---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 150ae4bb5d6e9ffcc976b0147502b4c16a022d4e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016152"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.InstalledAppsRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.InstalledAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).InstalledApps().Get(options)


```