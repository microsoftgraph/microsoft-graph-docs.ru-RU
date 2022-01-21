---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ab2fc7ef8a1acfd77dae477e80977b179cf6061
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118159"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatOperation -ChatId $chatId -TeamsAsyncOperationId $teamsAsyncOperationId

```