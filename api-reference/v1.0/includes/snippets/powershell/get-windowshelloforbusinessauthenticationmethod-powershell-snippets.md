---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e2882cd3f39445d85e80dfa4e8a94e37575c7af
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114568"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationWindowHello -UserId $userId -WindowsHelloForBusinessAuthenticationMethodId $windowsHelloForBusinessAuthenticationMethodId

```