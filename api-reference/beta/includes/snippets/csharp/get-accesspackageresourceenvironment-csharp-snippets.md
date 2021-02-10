---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7384375238ab548e74b641c432bf91360f62319f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceEnvironment = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceEnvironments["{accessPackageResourceEnvironmentId}"]
    .Request()
    .GetAsync();

```