---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a9f0dfa4e2cdcc3d3b836b1242ebf615bcbf503
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340381"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppManagementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
appManagementPolicyId := "appManagementPolicy-id"
graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).Patch(requestBody)


```