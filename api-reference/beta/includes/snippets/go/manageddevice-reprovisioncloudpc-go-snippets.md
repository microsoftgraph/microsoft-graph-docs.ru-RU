---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95668c2deeda85fad9af84a0b66f142f290b8df5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018514"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ReprovisionCloudPc().Post(options)


```