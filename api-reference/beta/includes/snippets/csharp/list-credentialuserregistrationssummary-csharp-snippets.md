---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b3d25d63822f504c5cd6efb29d59dbbcf4b803082bb6c866a1ee4ebba72b00f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationsSummaries = await graphClient.TenantRelationships.ManagedTenants.CredentialUserRegistrationsSummaries
    .Request()
    .GetAsync();

```