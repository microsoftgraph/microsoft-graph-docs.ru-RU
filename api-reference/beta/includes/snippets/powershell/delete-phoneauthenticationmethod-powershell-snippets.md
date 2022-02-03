---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6e342f26302e9358c43c82e3a2709774978f8bd
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349736"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Remove-MgUserAuthenticationPhoneMethod -UserId $userId -PhoneAuthenticationMethodId $phoneAuthenticationMethodId

```