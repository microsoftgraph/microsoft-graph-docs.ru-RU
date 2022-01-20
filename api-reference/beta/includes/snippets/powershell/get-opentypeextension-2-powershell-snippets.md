---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5acb505b9d72046139cc200efa10e83dfe8816f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112896"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgGroupEventExtension -GroupId $groupId -EventId $eventId -ExtensionId $extensionId

```