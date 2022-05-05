---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 462685fbf34430f5ae7472c467abdf3ae5f2cde7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205215"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).Cancel(unifiedRoleAssignmentScheduleRequest-id).Post(nil)


```