---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c1130ee8a42873c0ef4243d795acb91224c3139
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088855"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatInstalledApp -ChatId $chatId -ExpandProperty "teamsAppDefinition(`$expand=bot)" 

```