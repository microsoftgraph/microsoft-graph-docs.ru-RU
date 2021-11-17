---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e68edce7413af32ca428a2e7a16d008dbbff6055
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003380"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

cloudPcGalleryImageId := "cloudPcGalleryImage-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().GalleryImagesById(&cloudPcGalleryImageId).Get(options)


```