---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a470a6cdd0afacf8bdcba63f4c3762628bf5e0df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017968"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
teamsAsyncOperationId := "teamsAsyncOperation-id"
result, err := graphClient.ChatsById(&chatId).OperationsById(&teamsAsyncOperationId).Get(options)


```