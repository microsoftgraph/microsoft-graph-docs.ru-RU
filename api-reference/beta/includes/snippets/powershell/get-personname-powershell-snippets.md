---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c08f4c819c18971e5b9ce17e16cae45742310e7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349502"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileName -UserId $userId -PersonNameId $personNameId

```