---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c60f6985eca9039543b2c010ab5d6cd434da1e24ebe0db7be04d4f1629047d3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57318634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```