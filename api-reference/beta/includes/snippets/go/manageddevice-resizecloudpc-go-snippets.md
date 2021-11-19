---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc893d979d58fe8e092f011f3d41f78ae45d8113
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094028"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ResizeCloudPc().Post(options)


```