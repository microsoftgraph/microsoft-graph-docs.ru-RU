---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a303d1f0946f3a1393704838ff8879d40f98f5513c0f631b938e48c09c95dd7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackages = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .Request()
    .GetAsync();

```