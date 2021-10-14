---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: baff363206a830841fba23650ddfce4e5afb157cbfb1af0779e1bd264edb6e0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Devices["{device-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```