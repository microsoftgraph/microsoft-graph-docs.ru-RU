---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ea33f78a3d1eb0a5b84acedf5e1e4377c2e4ae2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128503"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "startsWith(appDisplayName,'Graph')",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().Get(options)


```