---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5690c042c3377106e5c27847686bccdd1b9f2f20
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalRiskDetectionId := "servicePrincipalRiskDetection-id"
result, err := graphClient.IdentityProtection().ServicePrincipalRiskDetectionsById(&servicePrincipalRiskDetectionId).Get()


```