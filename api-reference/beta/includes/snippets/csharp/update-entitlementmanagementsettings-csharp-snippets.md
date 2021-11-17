---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b0c6844d8ca377bef416d9601fd4db567c7c5b47f9df50056a3558cb55caba3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entitlementManagementSettings = new EntitlementManagementSettings
{
    ExternalUserLifecycleAction = "None"
};

await graphClient.IdentityGovernance.EntitlementManagement.Settings
    .Request()
    .UpdateAsync(entitlementManagementSettings);

```