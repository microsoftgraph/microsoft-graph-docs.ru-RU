---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a1b0855025805c9548a919512f92ea1322778fb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341422"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChildFoldersRequestBuilderGetQueryParameters{
    IncludeHiddenFolders: true,
}
options := &msgraphsdk.ChildFoldersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().GetWithRequestConfigurationAndResponseHandler(options, nil)


```