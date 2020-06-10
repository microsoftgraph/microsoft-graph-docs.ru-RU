---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ad2dd27c0e9b4626a43f9a9024a6629bdf71254
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684681"
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

await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```