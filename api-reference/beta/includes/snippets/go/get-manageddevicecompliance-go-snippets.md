---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff632759a1169f09a57d1ae52d42d7ec945ac53b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002897"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

managedDeviceComplianceId := "managedDeviceCompliance-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagedDeviceCompliancesById(&managedDeviceComplianceId).Get(options)


```