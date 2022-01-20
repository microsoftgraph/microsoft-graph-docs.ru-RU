---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8de88cc31effe61679a06ecfc73d5f24b2bc8c25
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106591"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "name-value"
    IsDefault = $false
}

New-MgOnPremisePublishingProfileConnectorGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```