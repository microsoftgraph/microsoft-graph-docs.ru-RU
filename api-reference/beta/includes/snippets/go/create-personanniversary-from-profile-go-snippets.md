---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d66a97c91e7639f1e8b022576afd67a79c5498e4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340054"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnualEvent()
type := "birthday"
requestBody.SetType(&type)
date := "1980-01-08"
requestBody.SetDate(&date)
result, err := graphClient.Me().Profile().Anniversaries().Post(requestBody)


```