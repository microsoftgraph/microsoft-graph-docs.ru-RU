---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ddacca20244bf1612c60eb0b1ce2801245fb5ef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351865"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    DisplayName = "Family"
}

# A UPN can also be used as -UserId.
New-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```