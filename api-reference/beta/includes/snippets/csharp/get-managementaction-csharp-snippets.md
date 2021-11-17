---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a632689071c79b2d4fb8b36346451b9d84c2f0b4c7061c73a4d0474f86e91e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementAction = await graphClient.TenantRelationships.ManagedTenants.ManagementActions["{managedTenants.managementAction-id}"]
    .Request()
    .GetAsync();

```