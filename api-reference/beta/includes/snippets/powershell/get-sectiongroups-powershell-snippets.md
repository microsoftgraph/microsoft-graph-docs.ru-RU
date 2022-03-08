---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82261c2efbed6fe0de59f26b1050bf84224a2fae
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331967"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteSectionGroup -UserId $userId -SectionGroupId $sectionGroupId

```