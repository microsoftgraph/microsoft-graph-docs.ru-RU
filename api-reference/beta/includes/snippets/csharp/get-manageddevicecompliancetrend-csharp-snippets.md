---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa9183ebf77f4a5dac5a400d7059e16b0adba3b5c7acd792d44a2501e7f64828
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceComplianceTrend = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceComplianceTrends["{managedTenants.managedDeviceComplianceTrend-id}"]
    .Request()
    .GetAsync();

```