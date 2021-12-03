---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 206a72a7be8bdae98c847ed146cdaf7c68db0fda
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295002"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Get(nil)


```