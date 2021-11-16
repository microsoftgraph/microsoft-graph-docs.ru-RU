---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e4f9ee5e4cfde7c37931abd3a7cd09917def854
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975404"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PoliciesRequestBuilderGetQueryParameters{
    Filter: "displayName%20eq%20'SimplePolicy1'%20or%20displayName%20eq%20'SimplePolicy2'",
}
options := &msgraphsdk.PoliciesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Get(options)


```