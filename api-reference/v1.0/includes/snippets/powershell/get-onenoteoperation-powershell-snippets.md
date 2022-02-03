---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 077ff50e24ba192ae2ef213ae7ba0490c0102007
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349984"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteOperation -UserId $userId -OnenoteOperationId $onenoteOperationId

```