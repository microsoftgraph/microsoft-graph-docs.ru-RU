---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 382f401d3d0355fc7ca9f0eb8b6cda9ab5a59748
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342118"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEntitlementManagementSettings()
externalUserLifecycleAction := "None"
requestBody.SetExternalUserLifecycleAction(&externalUserLifecycleAction)
graphClient.IdentityGovernance().EntitlementManagement().Settings().Patch(requestBody)


```