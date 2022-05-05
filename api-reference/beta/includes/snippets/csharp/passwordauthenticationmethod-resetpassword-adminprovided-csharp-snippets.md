---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ca5965f0822ca4c5ed76df9ae0816162e6fb061
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newPassword = "Cuyo5459";

await graphClient.Users["{user-id}"].Authentication.PasswordMethods["{passwordAuthenticationMethod-id}"]
    .ResetPassword(newPassword,null)
    .Request()
    .PostAsync();

```