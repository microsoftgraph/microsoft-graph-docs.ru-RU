---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97a9aabe11cd85d558976dc2e501e99bc0bc8b36
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "CN=customDisplayName"
requestBody.SetDisplayName(&displayName)
endDateTime, err := time.Parse(time.RFC3339, "2024-01-25T00:00:00Z")
requestBody.SetEndDateTime(&endDateTime)
options := &msgraphsdk.AddTokenSigningCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AddTokenSigningCertificate().Post(options)


```