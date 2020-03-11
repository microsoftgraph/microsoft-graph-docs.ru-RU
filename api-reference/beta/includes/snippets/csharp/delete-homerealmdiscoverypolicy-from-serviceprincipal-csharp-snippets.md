---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e0ff63c7a9905778daaa9a1149cfbc87c3cd62be
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589018"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```