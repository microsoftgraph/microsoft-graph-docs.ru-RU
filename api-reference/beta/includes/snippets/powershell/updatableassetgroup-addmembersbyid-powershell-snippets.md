---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00166d6647b6c70f4b25cda842ca95a2fcf0f84e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349007"
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

Add-MgWindowsUpdatesUpdatableAssetMemberById -UpdatableAssetId $updatableAssetId -BodyParameter $params

```