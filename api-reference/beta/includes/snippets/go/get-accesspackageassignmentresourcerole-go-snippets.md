---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 515734c4281f051bfe0eb5b1c885b454391cb8e7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294610"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentResourceRoleId := "accessPackageAssignmentResourceRole-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentResourceRolesById(&accessPackageAssignmentResourceRoleId).Get(nil)


```