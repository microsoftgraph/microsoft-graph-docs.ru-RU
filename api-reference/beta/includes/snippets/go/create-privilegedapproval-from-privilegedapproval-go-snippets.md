---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 38abcf2fbd3ca0a02320e0f59127bf8c24ceb7ef
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314817"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrivilegedApproval()
userId := "userId-value"
requestBody.SetUserId(&userId)
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
approvalType := "approvalType-value"
requestBody.SetApprovalType(&approvalType)
approvalState := "approvalState-value"
requestBody.SetApprovalState(&approvalState)
approvalDuration := "datetime-value"
requestBody.SetApprovalDuration(&approvalDuration)
result, err := graphClient.PrivilegedApproval().Post(requestBody)


```