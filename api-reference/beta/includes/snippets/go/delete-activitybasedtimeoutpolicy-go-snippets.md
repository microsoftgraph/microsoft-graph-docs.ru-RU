---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db255bce325200bd4e398f38e7b8de6973e13b6e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340414"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Delete()


```