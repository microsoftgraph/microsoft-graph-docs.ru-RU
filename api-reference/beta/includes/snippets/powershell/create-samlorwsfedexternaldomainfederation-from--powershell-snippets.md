---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6b316830f0d76bc201b4b7e49ec972715701a04
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099031"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.type" = "microsoft.graph.samlOrWsFedExternalDomainFederation"
    IssuerUri = "https://contoso.com/issuerUri"
    DisplayName = "contoso display name"
    MetadataExchangeUri = "https://contoso.com/metadataExchangeUri"
    PassiveSignInUri = "https://contoso.com/signin"
    PreferredAuthenticationProtocol = "wsFed"
    Domains = @(
        @{
            "@odata.type" = "microsoft.graph.externalDomainName"
            Id = "contoso.com"
        }
    )
    SigningCertificate = "MIIDADCCAeigAwIBAgIQEX41y8r6"
}

New-MgDirectoryFederationConfiguration -BodyParameter $params

```