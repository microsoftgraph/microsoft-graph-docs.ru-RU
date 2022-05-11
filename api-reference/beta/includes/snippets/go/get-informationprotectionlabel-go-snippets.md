---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c0bdb87a2705bc8401418cc4cefdd04517f80338
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340055"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

informationProtectionLabelId := "informationProtectionLabel-id"
result, err := graphClient.Me().InformationProtection().Policy().LabelsById(&informationProtectionLabelId).Get()


```