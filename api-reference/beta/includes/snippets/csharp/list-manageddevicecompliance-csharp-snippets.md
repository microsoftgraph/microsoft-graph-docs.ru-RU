---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af1e30e16c3ac69ca9d04c67459cae63617408920e181626477adbf4c49350e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceCompliances = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceCompliances
    .Request()
    .GetAsync();

```