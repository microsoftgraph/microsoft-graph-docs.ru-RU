---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2095b8b6862522960542dc53af5339186247d1a4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126672"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "endswith(mail,'a@contoso.com')" -Sort "userPrincipalName" -CountVariable CountVar -ConsistencyLevel eventual 


```