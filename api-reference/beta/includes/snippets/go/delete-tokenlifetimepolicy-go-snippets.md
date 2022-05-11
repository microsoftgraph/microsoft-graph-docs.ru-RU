---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 38a57ea18b0a285b5aaf0f38ecb59344db5f1365
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343173"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Delete()


```