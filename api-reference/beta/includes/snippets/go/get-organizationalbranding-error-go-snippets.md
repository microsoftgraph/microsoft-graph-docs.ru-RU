---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca665bdc640bd291d4bd46d73a7bf98a564a9016
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980477"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "Accept-Language": "0"
}
options := &msgraphsdk.BrandingRequestBuilderGetOptions{
    H: headers,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Get(options)


```