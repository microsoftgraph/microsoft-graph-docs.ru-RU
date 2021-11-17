---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b6aae6c4b25117664e63ddda77c0e203945574e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleEligibilityScheduleRequestId := "unifiedRoleEligibilityScheduleRequest-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequestsById(&unifiedRoleEligibilityScheduleRequestId).Get(options)


```