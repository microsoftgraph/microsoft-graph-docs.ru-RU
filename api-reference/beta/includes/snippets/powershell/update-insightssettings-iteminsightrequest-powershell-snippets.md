---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca3871cdec5b270678f25c2c8d63f0bc5bb506bc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096426"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgOrganizationSettingItemInsight -OrganizationId $organizationId -BodyParameter $params

```