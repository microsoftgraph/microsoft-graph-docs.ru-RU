---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2f0abbc51a9bf61d4934c86d209cddf9b38a32e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125138"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    "@odata.type" = "#microsoft.graph.windowsUpdates.updatableAssetGroup"
}

New-MgWindowsUpdatesUpdatableAsset -BodyParameter $params

```