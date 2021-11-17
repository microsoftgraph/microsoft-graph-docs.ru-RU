---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9643c6668608bb8acfa25755fea4f1fc2e29d30c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerId := "printer-id"
printTaskTriggerId := "printTaskTrigger-id"
graphClient.Print().PrintersById(&printerId).TaskTriggersById(&printTaskTriggerId).Delete(options)


```