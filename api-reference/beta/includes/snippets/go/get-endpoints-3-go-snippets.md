---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0166c335f882f251e162232946c2b0077b19759b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343404"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Print().Reports().DailyPrintUsageByPrinter().Get()


```