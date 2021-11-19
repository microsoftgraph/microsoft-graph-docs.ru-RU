---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7675f470b01959580cffe92aaa1aac37ed4bac04
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089152"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewScopedRoleMembership()
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
roleMemberInfo := msgraphsdk.NewIdentity()
requestBody.SetRoleMemberInfo(roleMemberInfo)
id := "id-value"
roleMemberInfo.SetId(&id)
options := &msgraphsdk.ScopedRoleMembersRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembers().Post(options)


```