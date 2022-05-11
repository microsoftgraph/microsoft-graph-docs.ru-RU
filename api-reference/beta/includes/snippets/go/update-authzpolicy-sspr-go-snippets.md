---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25cda0d79a583188ce534209364b533ee8ccf859
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342207"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowedToUseSSPR := true
requestBody.SetAllowedToUseSSPR(&allowedToUseSSPR)
authorizationPolicyId := "authorizationPolicy-id"
graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(requestBody)


```