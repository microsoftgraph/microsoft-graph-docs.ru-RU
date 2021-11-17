---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ea6812bf73b979a19d67dd53f865d14d6052400f82a098dfbeba3caadd09fbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsProtectionStates = await graphClient.TenantRelationships.ManagedTenants.WindowsProtectionStates
    .Request()
    .GetAsync();

```