---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc105bf86fcea92889123c39b7cf29b06f7373df
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339488"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    EntityType = "Group"
    DisplayName = "Myprefix_test_mysuffix"
    MailNickname = "Myprefix_test_mysuffix"
    OnBehalfOfUserId = "onBehalfOfUserId-value"
}

Test-MgDirectoryObjectProperty -BodyParameter $params

```