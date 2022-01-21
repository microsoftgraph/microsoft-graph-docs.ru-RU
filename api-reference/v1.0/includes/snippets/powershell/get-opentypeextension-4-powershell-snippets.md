---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ba2e41555b60d01438b4b61f53f0d3ddc0b6729
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134621"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupThreadPostExtension -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -ExtensionId $extensionId

```