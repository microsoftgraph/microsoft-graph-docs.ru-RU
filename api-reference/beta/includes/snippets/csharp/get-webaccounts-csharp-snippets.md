---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1cbee88b9c889ef09e24598818ab2c85d67b46d72f49edec0c3fd33c84b41267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57267799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccounts = await graphClient.Me.Profile.WebAccounts
    .Request()
    .GetAsync();

```