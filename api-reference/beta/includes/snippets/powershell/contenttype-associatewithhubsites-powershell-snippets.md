---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87df2842f647687f934d2241b386be37e164a42d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502488"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    HubSiteUrls = @(
        "https://graph.microsoft.com/beta/sites/id"
    )
    PropagateToExistingLists = $false
}

Join-MgSiteContentTypeWithHubSite -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```