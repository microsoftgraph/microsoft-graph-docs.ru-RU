---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ceb642c7d726c0579fc19894a70cd66016d17ab
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805698"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = new PhoneAuthenticationMethod
{
    PhoneNumber = "+1 2065555555",
    PhoneType = AuthenticationPhoneType.Mobile
};

await graphClient.Me.Authentication.PhoneMethods
    .Request()
    .AddAsync(phoneAuthenticationMethod);

```