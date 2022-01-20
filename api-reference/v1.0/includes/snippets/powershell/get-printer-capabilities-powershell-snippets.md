---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a6fe771ae3f35473c85817b0226f1d050a7bd14a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135776"
---
```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

Get-MgPrintPrinter -PrinterId $printerId -Property "id,displayName,capabilities" 

```