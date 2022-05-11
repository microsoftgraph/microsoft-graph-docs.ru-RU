---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60f4c0921a7e88881b69e7a960873e44f79e352c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343502"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantId := "tenant-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsById(&tenantId).OffboardTenant(tenant-id).Post()


```