---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb6b04e5afe2791acc5b27345410f50522e7d289
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978289"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

fido2AuthenticationMethodId := "fido2AuthenticationMethod-id"
result, err := graphClient.Me().Authentication().Fido2MethodsById(&fido2AuthenticationMethodId).Get(options)


```