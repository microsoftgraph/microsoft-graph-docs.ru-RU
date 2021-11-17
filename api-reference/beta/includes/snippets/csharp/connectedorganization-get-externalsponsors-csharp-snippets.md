---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6417932c24bfd521d39f1aee89e7686524d32cefebd035cb9d33ac6a0b718d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].ExternalSponsors
    .Request()
    .GetAsync();

```