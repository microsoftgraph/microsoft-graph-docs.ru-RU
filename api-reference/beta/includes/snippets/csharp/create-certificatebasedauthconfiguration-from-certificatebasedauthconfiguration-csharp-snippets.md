---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 919ff9caab7d0aca188a1d306632dfe392db97de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795033"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration
{
    CertificateAuthorities = new List<CertificateAuthority>()
    {
        new CertificateAuthority
        {
            IsRootAuthority = true,
            Certificate = Encoding.ASCII.GetBytes("Binary")
        }
    }
};

await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```