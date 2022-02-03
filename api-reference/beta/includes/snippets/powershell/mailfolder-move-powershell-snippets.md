---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68dcc51ad2a2588baa9cb97fde6a8670c8d26928
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346548"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    DestinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Move-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```