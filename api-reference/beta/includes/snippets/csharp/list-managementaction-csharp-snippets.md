---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 143d37585e051a35ab5f70264fc9a6f7720ef1ff8dd9a1a702d7841fb57a8e83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActions = await graphClient.TenantRelationships.ManagedTenants.ManagementActions
    .Request()
    .GetAsync();

```