---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: acfb61d16c4af405c8eeb99dd2d62ebb54fd0d4c
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225412"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
userAccountType := "administrator"
requestBody.SetUserAccountType(&userAccountType)
options := &msgraphsdk.ChangeUserAccountTypeRequestBuilderPostOptions{
    Body: requestBody,
}
cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).ChangeUserAccountType().Post(options)


```