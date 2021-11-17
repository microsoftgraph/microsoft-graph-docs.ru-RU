---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 917ea4d3377319e8d8af0721b32fbb539e3c5d18
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988910"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).Cancel().Post(options)


```