---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b4baed148148278ff69dc7ca491aa4197d51105
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019898"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ContentRequestBuilderGetQueryParameters{
    Format: "%7Bformat%7D",
}
options := &msgraphsdk.ContentRequestBuilderGetOptions{
    Q: requestParameters,
}
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Content().Get(options)


```