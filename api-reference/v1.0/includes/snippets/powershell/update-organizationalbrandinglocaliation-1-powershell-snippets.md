---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 389a3e0487b24fb8e54a440dfaeb69e35ebd0f34
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126165"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    SignInPageText = "Default"
    UsernameHintText = "DefaultHint"
}

Update-MgOrganizationBranding -OrganizationId $organizationId -BodyParameter $params

```