---
title: Создание маркеров подтверждения владения для смены ключей
description: В рамках подтверждения запроса для методов addKey и removeKey требуется маркер подтверждения владения. В этом документе приведены инструкции по созданию маркера подтверждения владения.
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: de27890f9e822f3cc75d1e8a1007794a0e70bf8c
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086741"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a><span data-ttu-id="0ad24-104">Создание маркеров подтверждения владения для смены ключей</span><span class="sxs-lookup"><span data-stu-id="0ad24-104">Generating proof of possession tokens for rolling keys</span></span>

<span data-ttu-id="0ad24-105">Вы можете использовать методы **addKey** и **removeKey**, определенные в ресурсах [application](/graph/api/resources/application?view=graph-rest-1.0) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0), для программной смены ключей с истекающим сроком действия.</span><span class="sxs-lookup"><span data-stu-id="0ad24-105">You can use the **addKey** and **removeKey** methods defined on the [application](/graph/api/resources/application?view=graph-rest-1.0) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) resources to roll expiring keys programmatically.</span></span>

<span data-ttu-id="0ad24-106">В рамках подтверждения запроса для этих методов проверяется подтверждение владения существующего ключа перед вызовом этих методов.</span><span class="sxs-lookup"><span data-stu-id="0ad24-106">As part of the request validation for these methods, a proof of possession of an existing key is verified before the methods can be invoked.</span></span> <span data-ttu-id="0ad24-107">Подтверждение представляется в виде самозаверяющего маркера JWT.</span><span class="sxs-lookup"><span data-stu-id="0ad24-107">The proof is represented by a self-signed JWT token.</span></span> <span data-ttu-id="0ad24-108">Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения.</span><span class="sxs-lookup"><span data-stu-id="0ad24-108">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="0ad24-109">Срок действия маркера не должен превышать 10 минут.</span><span class="sxs-lookup"><span data-stu-id="0ad24-109">The token lifespan should not exceed 10 minutes.</span></span>

> <span data-ttu-id="0ad24-110">**Примечание.** Приложения без существующих действительных сертификатов (сертификаты еще не добавлены или истек срок действия всех сертификатов) не смогут использовать это служебное действие.</span><span class="sxs-lookup"><span data-stu-id="0ad24-110">**Note:** Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="0ad24-111">Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](/graph/api/application-update?view=graph-rest-v1.0).</span><span class="sxs-lookup"><span data-stu-id="0ad24-111">You can use the [Update application](/graph/api/application-update?view=graph-rest-v1.0) operation to perform an update instead.</span></span>

<span data-ttu-id="0ad24-112">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="0ad24-112">The token should contain the following claims:</span></span>

- <span data-ttu-id="0ad24-113">`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="0ad24-113">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span>
- <span data-ttu-id="0ad24-114">`iss` — издателем должен быть __ObjectId__ Azure AD приложения, выполняющего вызов (а не applicationId или clientId).</span><span class="sxs-lookup"><span data-stu-id="0ad24-114">`iss` - Issuer needs to be the Azure AD __ObjectId__  of the application that is making the call (not the applicationId or clientId).</span></span>
- <span data-ttu-id="0ad24-115">`nbf` — вовремя.</span><span class="sxs-lookup"><span data-stu-id="0ad24-115">`nbf` - Not before time.</span></span>
- <span data-ttu-id="0ad24-116">`exp` — сроком действия должно быть значение "nbf" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="0ad24-116">`exp` - Expiration time should be "nbf" + 10 mins.</span></span>

<span data-ttu-id="0ad24-117">Вы можете использовать следующий пример кода, чтобы создать маркер подтверждения владения.</span><span class="sxs-lookup"><span data-stu-id="0ad24-117">You can use the following code example to generate this proof of possession token.</span></span>

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
