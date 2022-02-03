---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c353ec8af81a3a3dc3f8863b9cacdd8b872fa734
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350418"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationPasswordlessMicrosoftAuthenticatorMethod -UserId $userId -PasswordlessMicrosoftAuthenticatorAuthenticationMethodId $passwordlessMicrosoftAuthenticatorAuthenticationMethodId

```