---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b744e5b42cfef6deaa19eb996856cc6ccd4d3d2f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295386"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
microsoftAuthenticatorAuthenticationMethodId := "microsoftAuthenticatorAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().MicrosoftAuthenticatorMethodsById(&microsoftAuthenticatorAuthenticationMethodId).Delete(nil)


```