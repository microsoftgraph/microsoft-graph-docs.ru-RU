---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 343960dc6a8c3d90db3e40a651f88e988820906d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340484"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRoleScope()
accessPackageResourceRole := msgraphsdk.NewAccessPackageResourceRole()
requestBody.SetAccessPackageResourceRole(accessPackageResourceRole)
originId := "4"
accessPackageResourceRole.SetOriginId(&originId)
originSystem := "SharePointOnline"
accessPackageResourceRole.SetOriginSystem(&originSystem)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
accessPackageResourceRole.SetAccessPackageResource(accessPackageResource)
id := "53c71803-a0a8-4777-aecc-075de8ee3991"
accessPackageResource.SetId(&id)
accessPackageResourceScope := msgraphsdk.NewAccessPackageResourceScope()
requestBody.SetAccessPackageResourceScope(accessPackageResourceScope)
id := "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
accessPackageResourceScope.SetId(&id)
originId := "https://microsoft.sharepoint.com/portals/Community"
accessPackageResourceScope.SetOriginId(&originId)
originSystem := "SharePointOnline"
accessPackageResourceScope.SetOriginSystem(&originSystem)
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).AccessPackageResourceRoleScopes().Post(requestBody)


```