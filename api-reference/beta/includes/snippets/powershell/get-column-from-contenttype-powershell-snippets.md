---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3cfed425b501bd75bcf6d0ab902249f20b293e8b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125943"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId -ColumnDefinitionId $columnDefinitionId

```