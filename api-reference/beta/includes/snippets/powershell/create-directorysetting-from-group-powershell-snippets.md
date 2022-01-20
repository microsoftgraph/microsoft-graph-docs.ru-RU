---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f7e90806b5bd58deb799e51cec0c96524f4cf4e4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135511"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
}

New-MgGroupSetting -GroupId $groupId -BodyParameter $params

```