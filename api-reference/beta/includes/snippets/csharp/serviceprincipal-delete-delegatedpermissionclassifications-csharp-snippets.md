---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86ec6b58f42e7456e5e672e02451554d5ac1347bc3dd9685fdbe6a1996324572
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].DelegatedPermissionClassifications["{delegatedPermissionClassification-id}"]
    .Request()
    .DeleteAsync();

```