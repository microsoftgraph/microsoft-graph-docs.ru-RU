---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 361afd7ee8f3651fc7c4177e8d42811e9da29e15
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121708"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Labels = @(
        @{
            Name = "changedLabel"
            LanguageTag = "en-US"
            IsDefault = $true
        }
    )
}

Update-MgSiteTermStoreSetTerm -SiteId $siteId -SetId $setId -TermId $termId -BodyParameter $params

```