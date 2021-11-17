---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6bf19733bae217dd48352886f98a567fec6f4251
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
webUrl := "webUrl value"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.GetNotebookFromWebUrlRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Onenote().Notebooks().GetNotebookFromWebUrl().Post(options)


```