---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be30755d60da574dd88c61be237a1d0261b7a44909cf09f5e9e848ff5a71b170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealth = await graphClient.Admin.ServiceAnnouncement.HealthOverviews["{serviceHealth-id}"]
    .Request()
    .GetAsync();

```