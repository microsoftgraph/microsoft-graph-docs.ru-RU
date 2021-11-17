---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d5b3af4d6e0ad7e6979463e21a3e6474cf1418c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.CompleteRequestBuilderPostOptions{
    H: headers,
}
outlookTaskId := "outlookTask-id"
result, err := graphClient.Me().Outlook().TasksById(&outlookTaskId).Complete().Post(options)


```