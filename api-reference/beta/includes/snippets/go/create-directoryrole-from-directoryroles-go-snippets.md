---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7240ca5272a44a13ee9ebf57bb167f3983f08df5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340145"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectoryRole()
roleTemplateId := "fe930be7-5e62-47db-91af-98c3a49a38b1"
requestBody.SetRoleTemplateId(&roleTemplateId)
result, err := graphClient.DirectoryRoles().Post(requestBody)


```