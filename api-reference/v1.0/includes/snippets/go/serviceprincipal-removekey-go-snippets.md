---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d947ca17d01f4f660350c939ef5ffdebd2fa9d5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342297"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
proof := "eyJ0eXAiOiJ..."
requestBody.SetProof(&proof)
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).RemoveKey(servicePrincipal-id).Post(requestBody)


```