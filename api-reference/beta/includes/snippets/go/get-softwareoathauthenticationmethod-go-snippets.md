---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6e358af3d7edcaf2842c79809f53b555be816f95
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341054"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Get()


```