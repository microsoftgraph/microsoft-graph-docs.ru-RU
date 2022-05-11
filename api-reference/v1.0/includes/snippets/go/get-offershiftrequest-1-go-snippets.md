---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a6ae0869a170a4d90e0d771f7588a5135e423cc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
offerShiftRequestId := "offerShiftRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OfferShiftRequestsById(&offerShiftRequestId).Get()


```