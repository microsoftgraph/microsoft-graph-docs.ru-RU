---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77a0f4d364a5a6a46f4423c4ebbef2aa2b0670ca
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224866"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userRegistrationDetailsId := "userRegistrationDetails-id"
result, err := graphClient.Reports().AuthenticationMethods().UserRegistrationDetailsById(&userRegistrationDetailsId).Get(nil)


```