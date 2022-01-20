---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 386adee4cfbcc66118c36ba514143861ee27525f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100239"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCase()
displayName := "My Case 1"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.CasesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Compliance().Ediscovery().Cases().Post(options)


```