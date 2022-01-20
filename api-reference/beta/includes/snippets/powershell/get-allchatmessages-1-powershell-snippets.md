---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4fc0ec909640dd31ef95f90c63430aae11d8a22b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100573"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatMessage -ChatId $chatId -Top 2 -Sort "createdDateTime" 

```