---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e66236627224619c5ec3ea084f908712c275464b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342940"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
openShiftChangeRequestId := "openShiftChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequestsById(&openShiftChangeRequestId).Get()


```