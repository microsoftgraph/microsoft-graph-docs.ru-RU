---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 509c4f0c39544d7ed6fd55c0f46a28529c70d498
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100658"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChat -ChatId $chatId -ExpandProperty "members" 

```