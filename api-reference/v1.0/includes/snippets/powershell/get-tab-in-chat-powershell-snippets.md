---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a586a02722f42e9f54865d5bf39b4a9dd1ab1896
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101502"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatTab -ChatId $chatId -TeamsTabId $teamsTabId -ExpandProperty "teamsApp" 

```