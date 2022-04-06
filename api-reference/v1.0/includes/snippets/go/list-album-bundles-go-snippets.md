---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c4528cd2350f44433d79e028b3a490037f7968b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757930"
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