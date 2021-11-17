---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81e5613cfb8d7c4251581fd6506226cfc91c0d7b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988076"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessReviewsRequestBuilderGetQueryParameters{
    Filter: "businessFlowTemplateId%20eq%20'6e4f3d20-c5c3-407f-9695-8460952bcc68'",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.AccessReviewsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AccessReviews().Get(options)


```