---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e84e38216f1bfc5e26439efc357df0efbac3e58
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117949"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Topic = "Group chat title update"
}

Update-MgChat -ChatId $chatId -BodyParameter $params

```