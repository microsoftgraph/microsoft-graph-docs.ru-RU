---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c8c02604cd5f061b03a0959fefefcafdde5e2dd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102022"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleId := "unifiedRoleAssignmentSchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentSchedulesById(&unifiedRoleAssignmentScheduleId).Get(options)


```