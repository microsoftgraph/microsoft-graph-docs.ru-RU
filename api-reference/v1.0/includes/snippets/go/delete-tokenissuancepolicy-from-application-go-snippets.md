---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d925b7bfb8334200b67e0d6d26e433b235cff38
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695546"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenIssuancePoliciesById(&tokenIssuancePolicyId).$ref().Delete()


```