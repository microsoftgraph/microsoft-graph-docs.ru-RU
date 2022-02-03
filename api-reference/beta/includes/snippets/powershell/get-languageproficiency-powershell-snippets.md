---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3170217cb3e0e876c00e543e062ac286b62d013
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352769"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId

```