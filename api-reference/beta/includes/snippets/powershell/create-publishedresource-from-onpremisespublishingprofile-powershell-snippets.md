---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 63302a089df5f4386a648f62ce05f23945889c9a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105569"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "New provisioning"
    ResourceName = "domain1.contoso.com"
}

New-MgOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```