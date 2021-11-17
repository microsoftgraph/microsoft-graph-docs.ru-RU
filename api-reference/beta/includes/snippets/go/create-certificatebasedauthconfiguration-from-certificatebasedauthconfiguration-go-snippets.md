---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9068eaa6c4de7f1a88c2c7d4901c33542c47d2f9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026969"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "certificateAuthorities":  []Object {
    }
}
options := &msgraphsdk.CertificateBasedAuthConfigurationRequestBuilderPostOptions{
    Body: requestBody,
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).CertificateBasedAuthConfiguration().Post(options)


```