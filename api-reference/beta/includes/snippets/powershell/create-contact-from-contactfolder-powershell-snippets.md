---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebd7186dc3cda10620d05a1d5e3ab0445055e025
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351448"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "parentFolderId-value"
    Birthday = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    FileAs = "fileAs-value"
    DisplayName = "displayName-value"
    GivenName = "givenName-value"
    Initials = "initials-value"
}

# A UPN can also be used as -UserId.
New-MgUserContactFolderContact -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```