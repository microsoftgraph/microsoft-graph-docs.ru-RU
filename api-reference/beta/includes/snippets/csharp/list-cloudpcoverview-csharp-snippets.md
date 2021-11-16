---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f645c4890fad36390f8975dba79f4a6e9ceae1011562b144197bc330d730a56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57190533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcsOverview = await graphClient.TenantRelationships.ManagedTenants.CloudPcsOverview
    .Request()
    .GetAsync();

```