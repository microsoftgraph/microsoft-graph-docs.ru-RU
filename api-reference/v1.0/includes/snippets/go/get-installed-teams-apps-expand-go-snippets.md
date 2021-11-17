---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a9803c1708203ebea3c7794f9a70332029cb544d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988517"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppInstallationRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.TeamsAppInstallationRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
result, err := graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Get(options)


```