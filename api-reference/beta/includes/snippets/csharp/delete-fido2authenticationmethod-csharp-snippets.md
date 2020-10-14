---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a204ca0809b35ba370255443668d61aacf588bd0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458510"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.Fido2Methods["_jpuR-TGZtk6aQCLF3BQjA2"]
    .Request()
    .DeleteAsync();

```