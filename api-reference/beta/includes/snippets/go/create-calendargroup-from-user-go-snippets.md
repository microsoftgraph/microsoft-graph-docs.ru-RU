---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a812297f6475ca4926cde8e876733411968f74e4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101881"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarGroup()
name := "Personal events"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CalendarGroups().Post(options)


```