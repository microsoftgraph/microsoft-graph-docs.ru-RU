---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b803cacef838d3485ef11fc8dd3bef091c4f7d9a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997652"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Get(options)


```