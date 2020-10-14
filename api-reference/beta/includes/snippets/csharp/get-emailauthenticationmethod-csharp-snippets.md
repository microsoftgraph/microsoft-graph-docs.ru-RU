---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 65d71c856d31b94d31a78fcf0ed75afa3c9e69eb
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailMethods = await graphClient.Me.Authentication.EmailMethods
    .Request()
    .GetAsync();

```