---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d3b8344a78fb369509167503ece203a35e563355
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentsById(&accessPackageAssignmentId).Get()


```