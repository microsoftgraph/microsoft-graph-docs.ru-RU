---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4bf5ffd0939923a1749f86816715563eeb5d400b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350180"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

# A UPN can also be used as -UserId.
Get-MgUserAgreementAcceptance -UserId $userId

```