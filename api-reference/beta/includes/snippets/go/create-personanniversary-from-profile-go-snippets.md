---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 787268dd9d3363367dd97b7fa8359102516c8ae2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088358"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnualEvent()
type := "birthday"
requestBody.SetType(&type)
date := "1980-01-08"
requestBody.SetDate(&date)
options := &msgraphsdk.AnniversariesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Anniversaries().Post(options)


```