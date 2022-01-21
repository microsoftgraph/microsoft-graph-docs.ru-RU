---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 02177edb8484673bb577c81e12a2844afe9d8d3f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127480"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPublication()
publisher := "International Association of Branding Management Publishing"
requestBody.SetPublisher(&publisher)
thumbnailUrl := "https://iabm.io/sdhdfhsdhshsd.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
options := &msgraphsdk.ItemPublicationRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPublicationId := "itemPublication-id"
graphClient.UsersById(&userId).Profile().PublicationsById(&itemPublicationId).Patch(options)


```