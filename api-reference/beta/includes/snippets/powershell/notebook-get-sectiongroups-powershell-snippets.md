---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6250e3f3d329131f0164ef0c22ac71422b47fcc2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351846"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebookSectionGroup -UserId $userId -NotebookId $notebookId

```