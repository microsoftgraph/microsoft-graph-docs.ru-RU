---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ffd3c079065c628447bb8b8a2d6a1d78a81f49b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120091"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Annotations = @(
        @{
            Localizations = @(
                @{
                    LanguageTag = "no-NB"
                    DisplayName = "Kostnads Senter"
                }
            )
        }
    )
}

Update-MgOrganizationSettingProfileCardProperty -OrganizationId $organizationId -ProfileCardPropertyId $profileCardPropertyId -BodyParameter $params

```