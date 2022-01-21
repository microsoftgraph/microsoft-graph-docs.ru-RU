---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1890e89a1e565c8533333ff394daeebaaa621d12
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129621"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgPrivilegedRoleRoleAssignment -Filter "isElevated eq true" 

```