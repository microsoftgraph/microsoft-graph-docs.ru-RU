---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 945841b73021feda6e09b58299aaefa9e169a97e
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var isSyncedFromOnPremises = false;

await graphClient.DirectoryObjects
    .GetAvailableExtensionProperties(isSyncedFromOnPremises)
    .Request()
    .PostAsync();

```