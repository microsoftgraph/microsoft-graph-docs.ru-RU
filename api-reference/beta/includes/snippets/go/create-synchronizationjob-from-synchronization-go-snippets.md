---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82ebf0c8524d3c3ed3df28fe4956970fe31e6331
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341889"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSynchronizationJob()
templateId := "BoxOutDelta"
requestBody.SetTemplateId(&templateId)
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().Jobs().Post(requestBody)


```