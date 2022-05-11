---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dfd7f957d1345e77e39e6bc754d68d1c952d0ac9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleInstanceId := "unifiedRoleAssignmentScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleInstancesById(&unifiedRoleAssignmentScheduleInstanceId).Get()


```