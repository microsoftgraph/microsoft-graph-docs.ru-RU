---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c60d373dd3c28fc034235f29f56f2a3c1477a018
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027817"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleEligibilityScheduleRequestId := "unifiedRoleEligibilityScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequestsById(&unifiedRoleEligibilityScheduleRequestId).Cancel().Post(options)


```