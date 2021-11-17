---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 52cb5efca47ad6aee2088ed72283043b4fde7139
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023022"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printUsageByPrinterId := "printUsageByPrinter-id"
result, err := graphClient.Reports().DailyPrintUsageByPrinterById(&printUsageByPrinterId).Get(options)


```