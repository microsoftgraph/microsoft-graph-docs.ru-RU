---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49aa2f46f3991d29cded9964d5a224217f142072
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439049"
---
```powershell

Import-Module Microsoft.Graph.Groups

Remove-MgGroupMemberByRef -GroupId $groupId -DirectoryObjectId $directoryObjectId

```