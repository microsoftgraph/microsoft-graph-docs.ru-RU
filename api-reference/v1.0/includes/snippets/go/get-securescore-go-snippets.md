---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 214b73aa02ef6eb81f927da329df0c8d476768a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

secureScoreId := "secureScore-id"
result, err := graphClient.Security().SecureScoresById(&secureScoreId).Get(options)


```