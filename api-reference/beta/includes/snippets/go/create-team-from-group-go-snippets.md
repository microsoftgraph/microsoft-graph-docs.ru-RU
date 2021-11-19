---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fc53e0cb44642110ece49ecc07ea7b0bf280e1a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097137"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeam()
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "group@odata.bind": "https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')",
}
options := &msgraphsdk.TeamsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Teams().Post(options)


```