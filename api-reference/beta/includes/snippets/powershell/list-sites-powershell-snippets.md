---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b00e69f4b84ba3e8c028d197b140ff6367224fd2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111731"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSite -Property "siteCollection,webUrl" -Filter "siteCollection/root ne null" 

```