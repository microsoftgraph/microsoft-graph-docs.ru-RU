---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 28b2afeebf480e178e93450d453af85c1bd5a019
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032718"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcDeviceImageId := "cloudPcDeviceImage-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().DeviceImagesById(&cloudPcDeviceImageId).Get(options)


```