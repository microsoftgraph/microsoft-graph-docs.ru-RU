---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 139f6ac74e9938520cc3f112b10287c8e6781d3ab8a4f228c7310ac25560e693
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.TenantRelationships.ManagedTenants.RiskyUsers
    .Request()
    .GetAsync();

```