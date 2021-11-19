---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b7dbc1f737906b3d0e1a796092307c93ccfcbd1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090804"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewPolicy()
isGroupOwnerManagementEnabled := true
requestBody.SetIsGroupOwnerManagementEnabled(&isGroupOwnerManagementEnabled)
options := &msgraphsdk.AccessReviewPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().AccessReviewPolicy().Patch(options)


```