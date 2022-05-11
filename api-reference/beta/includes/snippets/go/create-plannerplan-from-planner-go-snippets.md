---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3fb9dabaf286200f5f2ec19d9e6b313a90eb218c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342164"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerPlan()
container := msgraphsdk.NewPlannerPlanContainer()
requestBody.SetContainer(container)
url := "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
container.SetUrl(&url)
title := "title-value"
requestBody.SetTitle(&title)
result, err := graphClient.Planner().Plans().Post(requestBody)


```