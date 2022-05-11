---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 579c57af8f9a126902f75c0841e6c1e77df81488
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341906"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementActionTenantDeploymentStatusId := "managementActionTenantDeploymentStatus-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatusesById(&managementActionTenantDeploymentStatusId).Get()


```