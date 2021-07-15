---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2552e2cbd425a63de5b0a20df04f8e1996389e0e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440612"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantsDetailedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsDetailedInformation
    .Request()
    .GetAsync();

```