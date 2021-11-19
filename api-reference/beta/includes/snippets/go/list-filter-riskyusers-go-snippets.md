---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46204093de5617bc842833a2a85a30b4b169c515
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094735"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RiskyUsersRequestBuilderGetQueryParameters{
    Filter: "riskLevel%20eq%20microsoft.graph.riskLevel'medium'",
}
options := &msgraphsdk.RiskyUsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityProtection().RiskyUsers().Get(options)


```