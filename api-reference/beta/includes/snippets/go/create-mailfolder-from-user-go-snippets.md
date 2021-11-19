---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0a0b0c6f35ecd79978a2c30c21a25d150685ed19
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "Clutter"
requestBody.SetDisplayName(&displayName)
isHidden := true
requestBody.SetIsHidden(&isHidden)
options := &msgraphsdk.MailFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().MailFolders().Post(options)


```