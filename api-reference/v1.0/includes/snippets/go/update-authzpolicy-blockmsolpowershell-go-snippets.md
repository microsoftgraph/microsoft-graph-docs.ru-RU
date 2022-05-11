---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d992e1b43aa5bcdbbf4ec97d1b22423947cd9f05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340806"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
blockMsolPowerShell := true
requestBody.SetBlockMsolPowerShell(&blockMsolPowerShell)
graphClient.Policies().AuthorizationPolicy().Patch(requestBody)


```