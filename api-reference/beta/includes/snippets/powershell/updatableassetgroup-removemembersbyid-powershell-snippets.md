---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b3177eca134bd4e820a186d1456ede12908dae8e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343807"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    Ids = @(
        "String"
        "String"
        "String"
    )
    MemberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice"
}

Remove-MgWindowsUpdatesUpdatableAssetMemberById -UpdatableAssetId $updatableAssetId -BodyParameter $params

```