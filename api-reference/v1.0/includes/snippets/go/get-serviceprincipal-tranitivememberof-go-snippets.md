---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07506ce9d1cb84119e0bdf6cc02702322da6c253
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).TransitiveMemberOf().Get()


```