---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6967e42a98a23bfa69671f986a0130b1db775f63469b7f41c5687fda273ea51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethod = await graphClient.Me.Authentication.Methods["{authenticationMethod-id}"]
    .Request()
    .GetAsync();

```