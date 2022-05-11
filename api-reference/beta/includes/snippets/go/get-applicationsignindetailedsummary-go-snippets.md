---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c53fe7a79c0c0554d05ab8e546522ae7af997199
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationSignInDetailedSummaryId := "applicationSignInDetailedSummary-id"
result, err := graphClient.Reports().ApplicationSignInDetailedSummaryById(&applicationSignInDetailedSummaryId).Get()


```