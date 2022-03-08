---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44090f8858c487742774038f597e802bf7a0be80
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334599"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyServicePrincipalId := "riskyServicePrincipal-id"
result, err := graphClient.IdentityProtection().RiskyServicePrincipalsById(&riskyServicePrincipalId).History().Get(nil)


```