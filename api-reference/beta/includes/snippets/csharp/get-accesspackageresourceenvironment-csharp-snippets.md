---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e5a8c51aec0e7930e1e9319794b506a4f5438e64
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809456"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceEnvironment = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceEnvironments["{accessPackageResourceEnvironment-id}"]
    .Request()
    .GetAsync();

```