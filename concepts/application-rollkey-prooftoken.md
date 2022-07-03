---
title: Создание маркеров подтверждения владения для смены ключей
description: В рамках подтверждения запроса для методов addKey и removeKey требуется маркер подтверждения владения. В этом документе приведены инструкции по созданию маркера подтверждения владения.
ms.localizationpriority: high
ms.prod: applications
author: FaithOmbongi
ms.openlocfilehash: 495c0a86020ff463b0bb76ab89f4f6b367e3af8d
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609656"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>Создание маркеров подтверждения владения для смены ключей

Вы можете использовать методы **addKey** и **removeKey**, определенные в ресурсах [application](/graph/api/resources/application) и [servicePrincipal](/graph/api/resources/serviceprincipal), для программной смены ключей с истекающим сроком действия.

В рамках подтверждения запроса для этих методов проверяется подтверждение владения существующего ключа перед вызовом этих методов. Подтверждение представляется в виде самозаверяющего маркера JWT. Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения. Срок действия маркера не должен превышать 10 минут.

> **Примечание.** Приложения без существующих действительных сертификатов (сертификаты еще не добавлены или истек срок действия всех сертификатов) не смогут использовать это служебное действие. Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](/graph/api/application-update).

Маркер должен содержать следующие утверждения:

- `aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.
- `iss` — издателем должен быть __ObjectId__ Azure AD приложения, выполняющего вызов (а не applicationId или clientId).
- `nbf` — вовремя.
- `exp` — сроком действия должно быть значение "nbf" + 10 минут.

Вы можете использовать следующий пример кода, чтобы создать маркер подтверждения владения.

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

> **Примечание.** Подтверждение можно создать с помощью других средств, например PowerShell или подписи с использованием Azure KeyVault. Важно отметить, что символ заполнения "=" не должен включаться в полезные данные и заголовок JWT. В противном случае возвращается ошибка **Authentication_MissingOrMalformed**.
