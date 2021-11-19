---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 732f279a3886cd7168794d1e367355e8136532c5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101966"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalConnection()
id := "contosohr"
requestBody.SetId(&id)
name := "Contoso HR"
requestBody.SetName(&name)
description := "Connection to index Contoso HR system"
requestBody.SetDescription(&description)
options := &msgraphsdk.ConnectionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.External().Connections().Post(options)


```