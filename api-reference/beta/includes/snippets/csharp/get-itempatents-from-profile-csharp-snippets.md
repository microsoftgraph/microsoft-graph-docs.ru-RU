---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca1b158aa7c1ef3c6aa5d4d924681f402149e68377715f316f65d24ad838b943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var patents = await graphClient.Me.Profile.Patents
    .Request()
    .GetAsync();

```