---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 626bab63f9e6ec4e4b1767b30c76437e293db0b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342831"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarGroup()
name := "name-value"
requestBody.SetName(&name)
calendarGroupId := "calendarGroup-id"
graphClient.Me().CalendarGroupsById(&calendarGroupId).Patch(requestBody)


```