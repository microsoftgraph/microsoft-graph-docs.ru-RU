---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5261e5652c0c5402a478dc64cbf6fd6296721b182f62fccd7d7a3a9c85d8394
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicyCoverages = await graphClient.TenantRelationships.ManagedTenants.ConditionalAccessPolicyCoverages
    .Request()
    .GetAsync();

```