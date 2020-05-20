---
title: Создание пробных маркеров для использования для чередующихся ключей
description: В ходе проверки запросов для методов Аддкэй и Ремовекэй необходимо подтверждение маркера использования. В этом документе представлены рекомендации по созданию маркера для проверки подлинности.
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 516673b3f5ef318f1c2cc42778d8bec99471c630
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289653"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>Создание пробных маркеров для использования для чередующихся ключей

Вы можете использовать методы **аддкэй** и **ремовекэй** , определенные в ресурсах [Application](/graph/resources/application?view=graph-rest-v1.0) и [servicePrincipal](/graph/resources/serviceprincipal?view=graph-rest-v1.0) , для программного истечения срока действия ключа.

В рамках проверки запросов для этих методов проверяется наличие проверки на наличие существующего ключа перед вызовом этих методов. Проверка представляется с помощью маркера JWT с собственной подписью. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов приложения. Срок действия маркера не должен превышать 10 минут.

> **Примечание:** Приложения, у которых нет существующих действительных сертификатов (сертификаты не были добавлены до тех пор, или у всех сертификатов истек срок действия), не удастся использовать это действие службы. Вместо этого можно использовать операцию [обновления приложения](/graph/api/application-update?view=graph-rest-v1.0) для выполнения обновления.

Маркер должен содержать следующие утверждения:

- `aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .
- `iss`-Issuer должен быть __идентификатором__ приложения, осуществляющего вызов.
- `nbf`— Не до времени.
- `exp`— Срок действия должен быть "NBF" + 10 минут.

Вы можете использовать следующий пример кода для создания этого маркера для проверки подлинности.

```csharp
using System;
using System.Collections.Generic;
using System.Security.Cryptography.X509Certificates;
using Microsoft.IdentityModel.Tokens;
using Microsoft.IdentityModel.JsonWebTokens;

namespace MicrosoftIdentityPlatformProofTokenGenerator
{
    class Program
    {
        static void Main(string[] args)
        {
            // Configure the following
            string pfxFilePath = "<Path to your certificate file";
            string password = "<Certificate password>";
            string objectId = "<id of the application or servicePrincipal object>";

            // Get signing certificate
            X509Certificate2 signingCert = new X509Certificate2(pfxFilePath, password);

            // audience
            string aud = $"00000002-0000-0000-c000-000000000000";

            // aud and iss are the only required claims.
            var claims = new Dictionary<string, object>()
            {
                { "aud", aud },
                { "iss", objectId }
            };

            // token validity should not be more than 10 minutes
            var now = DateTime.UtcNow;
            var securityTokenDescriptor = new SecurityTokenDescriptor
            {
                Claims = claims,
                NotBefore = now,
                Expires = now.AddMinutes(10),
                SigningCredentials = new X509SigningCredentials(signingCert)
            };

            var handler = new JsonWebTokenHandler();
            var x = handler.CreateToken(securityTokenDescriptor);
            Console.WriteLine(x);
        }
    }
}
```
