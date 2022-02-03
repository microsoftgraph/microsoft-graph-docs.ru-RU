---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab28f871a69503fa293fcb38283a73c7bfb82a2b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346773"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    HubSiteUrls = @(
        "https://graph.microsoft.com/v1.0/sites/{site-id}"
    )
    PropagateToExistingLists = $false
}

Join-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```