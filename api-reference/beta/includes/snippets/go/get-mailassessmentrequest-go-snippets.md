---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 237f7c3230f2cdbe6b6110a389f96f9a82ef4163
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977510"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

threatAssessmentRequestId := "threatAssessmentRequest-id"
result, err := graphClient.InformationProtection().ThreatAssessmentRequestsById(&threatAssessmentRequestId).Get(options)


```