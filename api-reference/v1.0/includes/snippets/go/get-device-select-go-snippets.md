---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5dfb21a8121814bc8a4394b6ee4de905b3e17f5e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeviceRequestBuilderGetQueryParameters{
    Select: "id,extensionAttributes",
}
options := &msgraphsdk.DeviceRequestBuilderGetOptions{
    Q: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Get(options)


```