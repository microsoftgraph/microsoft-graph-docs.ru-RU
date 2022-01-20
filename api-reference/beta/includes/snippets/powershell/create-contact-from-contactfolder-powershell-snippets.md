---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 32d3aa2fbe43c630cd6d3dd6e2e4f91dc63ce286
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103679"
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

New-MgUserContactFolderContact -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```