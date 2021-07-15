---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 163783d2735c55105ca2323b074eccc86fe09930
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceComplianceTrend = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceComplianceTrends["{managedTenants.managedDeviceComplianceTrend-id}"]
    .Request()
    .GetAsync();

```