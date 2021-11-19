---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c4528cd2350f44433d79e028b3a490037f7968b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100740"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.BundlesRequestBuilderGetQueryParameters{
    Filter: "bundle/album%20ne%20null",
}
options := &msgraphsdk.BundlesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Drive().Bundles().Get(options)


```