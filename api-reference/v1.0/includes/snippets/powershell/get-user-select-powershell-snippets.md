---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e81e861c2850f02bc7844b6da6bdeb4075fd7bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121657"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -UserId $userId -Property "displayName,givenName,postalCode,identities" 

```