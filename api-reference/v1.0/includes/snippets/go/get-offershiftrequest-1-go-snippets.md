---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81b9927d3f32178dfbeea52f874d73e53ceef039
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295633"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
offerShiftRequestId := "offerShiftRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OfferShiftRequestsById(&offerShiftRequestId).Get(nil)


```