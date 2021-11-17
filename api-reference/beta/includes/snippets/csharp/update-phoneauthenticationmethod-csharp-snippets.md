---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ed952d64dfac38b8923a726c523ab920119341741fb7e709ac4149f69dacd33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = new PhoneAuthenticationMethod
{
    PhoneNumber = "+1 2065555554",
    PhoneType = AuthenticationPhoneType.Mobile
};

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .Request()
    .PutAsync(phoneAuthenticationMethod);

```