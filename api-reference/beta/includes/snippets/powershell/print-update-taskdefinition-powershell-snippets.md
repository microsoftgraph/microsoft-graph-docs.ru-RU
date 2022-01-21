---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b33c34e717d24d57366964b6db31417700156d86
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127189"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "Test TaskDefinitionName"
    CreatedBy = @{
        DisplayName = "Requesting App Display Name"
    }
}

Update-MgPrintTaskDefinition -PrintTaskDefinitionId $printTaskDefinitionId -BodyParameter $params

```