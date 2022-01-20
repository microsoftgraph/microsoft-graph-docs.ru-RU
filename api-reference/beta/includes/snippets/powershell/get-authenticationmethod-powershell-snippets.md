---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b6fd60549195c217b05478308158c81835cb2777
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114252"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationMethod -UserId $userId -AuthenticationMethodId $authenticationMethodId

```