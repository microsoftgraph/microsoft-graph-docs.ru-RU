---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5574d0646bbe5786bfb7e350b29590c6ad89a116
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132530"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgChatInstalledApp -ChatId $chatId -TeamsAppInstallationId $teamsAppInstallationId

```