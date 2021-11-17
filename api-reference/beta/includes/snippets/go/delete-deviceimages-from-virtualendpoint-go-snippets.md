---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a21eb46c2ec9c78ab4eed233e48aece9f25d9f56
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcDeviceImageId := "cloudPcDeviceImage-id"
graphClient.DeviceManagement().VirtualEndpoint().DeviceImagesById(&cloudPcDeviceImageId).Delete(options)


```