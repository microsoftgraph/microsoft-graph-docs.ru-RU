---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3de545dd7b3afafde243089b4298ad12d773bed7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088955"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcGalleryImageId := "cloudPcGalleryImage-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().GalleryImagesById(&cloudPcGalleryImageId).Get(options)


```