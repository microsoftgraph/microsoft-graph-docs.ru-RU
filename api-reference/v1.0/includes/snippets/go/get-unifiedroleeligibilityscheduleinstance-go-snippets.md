---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2931a61fe4a6496267320f5e2a4a51cc51c28cc2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65339976"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleInstanceId := "unifiedRoleEligibilityScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleInstancesById(&unifiedRoleEligibilityScheduleInstanceId).Get()


```