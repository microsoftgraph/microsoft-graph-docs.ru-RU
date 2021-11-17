---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbc03beb7ff614637a76f1eb94bec48e462aedca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Delete(options)


```