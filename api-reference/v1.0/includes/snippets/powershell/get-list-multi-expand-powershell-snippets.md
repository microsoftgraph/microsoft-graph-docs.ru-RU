---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0d9d195ac782a0cf20b1dc6d64c569eec502ba4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088581"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteList -SiteId $siteId -ListId $listId -Property "id,name,lastModifiedDateTime" -ExpandProperty "columns(select=name,description),items)" 

```