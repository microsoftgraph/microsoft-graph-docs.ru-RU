---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0be3abf81bc052ec4f61bb4917ab2c20f1179f5f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccounts = await graphClient.Me.Profile.WebAccounts
    .Request()
    .GetAsync();

```