---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba7a14d7fb277f9c49825e23d48d4040dcad9f28f512cfe04ca8e34c6e725fb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = await graphClient.Users["{user-id}"].Profile.Emails["{itemEmail-id}"]
    .Request()
    .GetAsync();

```