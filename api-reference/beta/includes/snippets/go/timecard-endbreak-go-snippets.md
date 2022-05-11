---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c14fcc995b27828f39fa5a4ad842e0898293c147
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340828"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
contentType := "text"
notes.SetContentType(&contentType)
content := "end break smaple notes"
notes.SetContent(&content)
requestBody.SetAdditionalData(map[string]interface{}{
    "atAprovedLocation": true,
}
teamId := "team-id"
timeCardId := "timeCard-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).EndBreak(team-id, timeCard-id).Post(requestBody)


```