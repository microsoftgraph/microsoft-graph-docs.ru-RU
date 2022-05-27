---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae9e1e31fa6cf43e45bda1e9edd05a731f4eb949
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicy()
requestBody.SetAdditionalData(map[string]interface{}{
    "allowedCloudEndpoints":  []String {
        "microsoftonline.us",
        "partner.microsoftonline.cn",
    }
}
graphClient.Policies().CrossTenantAccessPolicy().Patch(requestBody)


```