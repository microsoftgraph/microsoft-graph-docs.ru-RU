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
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a><span data-ttu-id="13a36-104">Создание пробных маркеров для использования для чередующихся ключей</span><span class="sxs-lookup"><span data-stu-id="13a36-104">Generating proof of possession tokens for rolling keys</span></span>

<span data-ttu-id="13a36-105">Вы можете использовать методы **аддкэй** и **ремовекэй** , определенные в ресурсах [Application](/graph/resources/application?view=graph-rest-v1.0) и [servicePrincipal](/graph/resources/serviceprincipal?view=graph-rest-v1.0) , для программного истечения срока действия ключа.</span><span class="sxs-lookup"><span data-stu-id="13a36-105">You can use the **addKey** and **removeKey** methods defined on the [application](/graph/resources/application?view=graph-rest-v1.0) and [servicePrincipal](/graph/resources/serviceprincipal?view=graph-rest-v1.0) resources to roll expiring keys programmatically.</span></span>

<span data-ttu-id="13a36-106">В рамках проверки запросов для этих методов проверяется наличие проверки на наличие существующего ключа перед вызовом этих методов.</span><span class="sxs-lookup"><span data-stu-id="13a36-106">As part of the request validation for these methods, a proof of possession of an existing key is verified before the methods can be invoked.</span></span> <span data-ttu-id="13a36-107">Проверка представляется с помощью маркера JWT с собственной подписью.</span><span class="sxs-lookup"><span data-stu-id="13a36-107">The proof is represented by a self-signed JWT token.</span></span> <span data-ttu-id="13a36-108">Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов приложения.</span><span class="sxs-lookup"><span data-stu-id="13a36-108">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="13a36-109">Срок действия маркера не должен превышать 10 минут.</span><span class="sxs-lookup"><span data-stu-id="13a36-109">The token lifespan should not exceed 10 minutes.</span></span>

> <span data-ttu-id="13a36-110">**Примечание:** Приложения, у которых нет существующих действительных сертификатов (сертификаты не были добавлены до тех пор, или у всех сертификатов истек срок действия), не удастся использовать это действие службы.</span><span class="sxs-lookup"><span data-stu-id="13a36-110">**Note:** Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="13a36-111">Вместо этого можно использовать операцию [обновления приложения](/graph/api/application-update?view=graph-rest-v1.0) для выполнения обновления.</span><span class="sxs-lookup"><span data-stu-id="13a36-111">You can use the [Update application](/graph/api/application-update?view=graph-rest-v1.0) operation to perform an update instead.</span></span>

<span data-ttu-id="13a36-112">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="13a36-112">The token should contain the following claims:</span></span>

- <span data-ttu-id="13a36-113">`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="13a36-113">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span>
- <span data-ttu-id="13a36-114">`iss`-Issuer должен быть __идентификатором__ приложения, осуществляющего вызов.</span><span class="sxs-lookup"><span data-stu-id="13a36-114">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span>
- <span data-ttu-id="13a36-115">`nbf`— Не до времени.</span><span class="sxs-lookup"><span data-stu-id="13a36-115">`nbf` - Not before time.</span></span>
- <span data-ttu-id="13a36-116">`exp`— Срок действия должен быть "NBF" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="13a36-116">`exp` - Expiration time should be "nbf" + 10 mins.</span></span>

<span data-ttu-id="13a36-117">Вы можете использовать следующий пример кода для создания этого маркера для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="13a36-117">You can use the following code example to generate this proof of possession token.</span></span>

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
