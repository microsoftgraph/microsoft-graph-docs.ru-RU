---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92821bead1dbdcdb39ba42f38222c3c8e332b816544a847d1151a0758b5b7fb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = new Domain
{
    IsDefault = true,
    SupportedServices = new List<String>()
    {
        "Email",
        "OfficeCommunicationsOnline"
    }
};

await graphClient.Domains["{domain-id}"]
    .Request()
    .UpdateAsync(domain);

```