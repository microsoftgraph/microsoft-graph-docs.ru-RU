---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95b7bc0f60af73a8d5472a94caf929c0bb092387ff0002d5ad70d1c40318d156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57308107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceCompliance = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceCompliances["{managedTenants.managedDeviceCompliance-id}"]
    .Request()
    .GetAsync();

```