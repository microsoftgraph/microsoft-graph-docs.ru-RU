---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e21635ce81b069ca9cd66b56f25662b816dfb5c3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117011"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
    DisplayName = "Test TaskDefinitionName"
    CreatedBy = @{
        DisplayName = "Requesting App Display Name"
    }
}

New-MgPrintTaskDefinition -BodyParameter $params

```