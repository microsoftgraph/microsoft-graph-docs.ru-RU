---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc6ffd54d038059b00f3682eece48b36942fea00
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.DirectReportsRequestBuilderPostOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).DirectReports().Post(options)


```