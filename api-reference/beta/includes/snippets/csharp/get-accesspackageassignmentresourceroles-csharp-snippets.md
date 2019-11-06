---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 872c922d02d45805aa15d35a66ee6f4e601ee809
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentResourceRoles
    .Request()
    .GetAsync();

```