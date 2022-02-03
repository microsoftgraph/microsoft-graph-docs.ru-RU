---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 28f691700037f643289f81cd052f47b5b69c9c77
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350249"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebook -UserId $userId -NotebookId $notebookId

```