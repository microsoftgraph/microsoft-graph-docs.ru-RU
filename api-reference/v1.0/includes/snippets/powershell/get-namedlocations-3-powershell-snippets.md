---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d67cb577fcbaa609686824fbcbcbe89bc7a3a75e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124915"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgIdentityConditionalAccessNamedLocation -Filter "createdDateTime ge 2019-09-01T00:00:00Z" 

```