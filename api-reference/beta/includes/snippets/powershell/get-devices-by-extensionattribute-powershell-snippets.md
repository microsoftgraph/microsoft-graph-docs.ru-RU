---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fbf3a2cd320ce06b3faa7e36c337cf7a72f52134
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133996"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDevice -Filter "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'" -CountVariable CountVar -ConsistencyLevel eventual 


```