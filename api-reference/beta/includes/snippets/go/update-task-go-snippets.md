---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ce28c253b0449cb4fbc60a860894bd766782503
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341448"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrintTask()
status := msgraphsdk.NewPrintTaskStatus()
requestBody.SetStatus(status)
state := "completed"
status.SetState(&state)
description := "completed"
status.SetDescription(&description)
printTaskDefinitionId := "printTaskDefinition-id"
printTaskId := "printTask-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).TasksById(&printTaskId).Patch(requestBody)


```