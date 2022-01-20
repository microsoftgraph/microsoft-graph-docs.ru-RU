---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71b0a390044a50434d3677a7584434ed571dba3d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113027"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section group name"
}

New-MgUserOnenoteNotebookSectionGroup -UserId $userId -NotebookId $notebookId -BodyParameter $params

```