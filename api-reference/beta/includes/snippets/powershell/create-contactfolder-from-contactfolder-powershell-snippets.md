---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ff1f56dad9906efa6fd13de5bd7d08d71c8cd1d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094326"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    DisplayName = "Family"
}

New-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```