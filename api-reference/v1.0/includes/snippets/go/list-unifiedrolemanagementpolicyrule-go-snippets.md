---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3421c9083b994bb6f7ec45a2f960418aa64293fe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341576"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleManagementPolicyId := "unifiedRoleManagementPolicy-id"
result, err := graphClient.Policies().RoleManagementPoliciesById(&unifiedRoleManagementPolicyId).Rules().Get()


```