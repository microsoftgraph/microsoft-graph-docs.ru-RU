---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a910391f1ef0ce8b9ae3d0ff7bce8f1ba001167a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132250"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    Event = "jobStarted"
    "Definition@odata.bind" = "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
}

New-MgPrintPrinterTaskTrigger -PrinterId $printerId -BodyParameter $params

```