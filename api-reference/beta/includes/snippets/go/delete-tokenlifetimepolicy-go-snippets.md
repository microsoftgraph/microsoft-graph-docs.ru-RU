---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c39b8e94fcc11eaf6a1070c7d026ab2bfd01c12c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416590"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenLifetimePolicyId := "tokenLifetimePolicy-id"
result, err := graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Delete(nil)


```