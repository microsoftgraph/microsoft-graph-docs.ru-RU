---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c396f4d06a35fe1aede9e17334f6693c71d11409
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340810"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowEmailVerifiedUsersToJoinOrganization := false
requestBody.SetAllowEmailVerifiedUsersToJoinOrganization(&allowEmailVerifiedUsersToJoinOrganization)
graphClient.Policies().AuthorizationPolicy().Patch(requestBody)


```