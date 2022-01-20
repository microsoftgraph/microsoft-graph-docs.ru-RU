---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8572efd109a81d9a880ccc06d055dad4f7e428c5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121553"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationWindowHello -UserId $userId -WindowsHelloForBusinessAuthenticationMethodId $windowsHelloForBusinessAuthenticationMethodId

```