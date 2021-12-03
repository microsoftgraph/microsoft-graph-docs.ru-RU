---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aeb1b4481fd1926f7053a39a59571c89248f4094
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295751"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

emailAuthenticationMethodId := "emailAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().EmailMethodsById(&emailAuthenticationMethodId).Get(nil)


```