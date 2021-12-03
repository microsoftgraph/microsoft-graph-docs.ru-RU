---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3e03b96bfaca4098f03a585cdfca117a4b26c444
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295692"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
windowsHelloForBusinessAuthenticationMethodId := "windowsHelloForBusinessAuthenticationMethod-id"
result, err := graphClient.UsersById(&userId).Authentication().WindowsHelloForBusinessMethodsById(&windowsHelloForBusinessAuthenticationMethodId).Get(nil)


```