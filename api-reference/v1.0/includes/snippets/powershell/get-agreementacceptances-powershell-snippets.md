---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4bf5ffd0939923a1749f86816715563eeb5d400b
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516000"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

# A UPN can also be used as -UserId.
Get-MgUserAgreementAcceptance -UserId $userId

```