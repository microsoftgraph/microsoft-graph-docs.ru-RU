---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 957d1ce0c31af7b669718811628a19bc527f87d1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var isSyncedFromOnPremises = true;

await graphClient.DirectoryObjects
    .GetAvailableExtensionProperties(isSyncedFromOnPremises)
    .Request()
    .PostAsync();

```