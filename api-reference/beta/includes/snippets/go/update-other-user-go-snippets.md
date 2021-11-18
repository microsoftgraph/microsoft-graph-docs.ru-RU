---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f048d240abd9e54dd83af71ee5d731013439a1e3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077296"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
requestBody.SetBusinessPhones( []String {
    "+1 425 555 0109",
}
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation)
options := &msgraphsdk.UserRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Patch(options)


```