---
title: 'servicePrincipal: addKey'
description: Добавление учетных данных ключа объекту servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2588a60333fa6a4d66cbbf682225d21dc5cfc476
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959496"
---
# <a name="serviceprincipal-addkey"></a><span data-ttu-id="73a6c-103">servicePrincipal: addKey</span><span class="sxs-lookup"><span data-stu-id="73a6c-103">servicePrincipal: addKey</span></span>

<span data-ttu-id="73a6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73a6c-105">Добавляет ключевые учетные данные [в службуPrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="73a6c-105">Adds a key credential to a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="73a6c-106">Этот метод наряду с [removeKey](serviceprincipal-removekey.md) может использоваться службойPrincipal для автоматизации проката истекающих ключей.</span><span class="sxs-lookup"><span data-stu-id="73a6c-106">This method along with [removeKey](serviceprincipal-removekey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="73a6c-107">[Создание службыPrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [Update servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления учетных данных для любой службыPrincipal с контекстом пользователя или без него.</span><span class="sxs-lookup"><span data-stu-id="73a6c-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="73a6c-108">В рамках проверки запроса для этого метода проверяется доказательство на наличие существующего ключа перед выполнением действия.</span><span class="sxs-lookup"><span data-stu-id="73a6c-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="73a6c-109">ServicePrincipals, у которых нет существующих действительных сертификатов (например, еще не добавлены сертификаты или истек срок действия всех сертификатов), не смогут использовать это действие службы.</span><span class="sxs-lookup"><span data-stu-id="73a6c-109">ServicePrincipals that don’t have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="73a6c-110">Для выполнения обновления можно использовать службу [UpdatePrincipal.](../api/serviceprincipal-update.md)</span><span class="sxs-lookup"><span data-stu-id="73a6c-110">[Update servicePrincipal](../api/serviceprincipal-update.md) can be used to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a6c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73a6c-111">Permissions</span></span>

|<span data-ttu-id="73a6c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73a6c-112">Permission type</span></span>      | <span data-ttu-id="73a6c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73a6c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73a6c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73a6c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="73a6c-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73a6c-115">None.</span></span>  |
|<span data-ttu-id="73a6c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73a6c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73a6c-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="73a6c-117">None.</span></span>    |
|<span data-ttu-id="73a6c-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="73a6c-118">Application</span></span> | <span data-ttu-id="73a6c-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73a6c-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="73a6c-120">СлужбаPrincipal не нуждается в специальном разрешении для сверки собственных ключей.</span><span class="sxs-lookup"><span data-stu-id="73a6c-120">A servicePrincipal does not need any specific permission to roll it's own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="73a6c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73a6c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="73a6c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73a6c-122">Request headers</span></span>

| <span data-ttu-id="73a6c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="73a6c-123">Name</span></span>           | <span data-ttu-id="73a6c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="73a6c-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="73a6c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73a6c-125">Authorization</span></span>  | <span data-ttu-id="73a6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73a6c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73a6c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73a6c-128">Content-Type</span></span>   | <span data-ttu-id="73a6c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73a6c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73a6c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73a6c-131">Request body</span></span>

<span data-ttu-id="73a6c-132">В теле запроса укажи следующие необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="73a6c-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="73a6c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="73a6c-133">Property</span></span>     | <span data-ttu-id="73a6c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="73a6c-134">Type</span></span>   |<span data-ttu-id="73a6c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="73a6c-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73a6c-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="73a6c-136">keyCredential</span></span> | [<span data-ttu-id="73a6c-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="73a6c-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="73a6c-138">Добавлены новые учетные данные ключа servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="73a6c-138">The new servicePrincipal key credential to add.</span></span> <span data-ttu-id="73a6c-139">__Тип,__ __использование и__ __ключ__ необходимые свойства для этого использования.</span><span class="sxs-lookup"><span data-stu-id="73a6c-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="73a6c-140">Поддерживаемые ключевые типы:</span><span class="sxs-lookup"><span data-stu-id="73a6c-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="73a6c-141">`AsymmetricX509Cert`: Использование должно быть `Verify` .</span><span class="sxs-lookup"><span data-stu-id="73a6c-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="73a6c-142">`X509CertAndPassword`: Использование должно быть `Sign`</span><span class="sxs-lookup"><span data-stu-id="73a6c-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="73a6c-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="73a6c-143">passwordCredential</span></span> | [<span data-ttu-id="73a6c-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="73a6c-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="73a6c-145">Требуется __установить только secretText,__ который должен содержать пароль для ключа.</span><span class="sxs-lookup"><span data-stu-id="73a6c-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="73a6c-146">Это свойство требуется только для ключей типа `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="73a6c-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="73a6c-147">Установите его в `null` противном случае.</span><span class="sxs-lookup"><span data-stu-id="73a6c-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="73a6c-148">доказательство</span><span class="sxs-lookup"><span data-stu-id="73a6c-148">proof</span></span> | <span data-ttu-id="73a6c-149">String</span><span class="sxs-lookup"><span data-stu-id="73a6c-149">String</span></span> | <span data-ttu-id="73a6c-150">Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами.</span><span class="sxs-lookup"><span data-stu-id="73a6c-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="73a6c-151">Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов службыPrincipal.</span><span class="sxs-lookup"><span data-stu-id="73a6c-151">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="73a6c-152">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="73a6c-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="73a6c-153">`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="73a6c-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="73a6c-154">`iss` - Эмитент должен быть __id__  службыPrincipal, которая делает вызов.</span><span class="sxs-lookup"><span data-stu-id="73a6c-154">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="73a6c-155">`nbf` — вовремя.</span><span class="sxs-lookup"><span data-stu-id="73a6c-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="73a6c-156">`exp` — сроком действия должно быть значение "nbf" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="73a6c-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="73a6c-157">Вот пример [кода,](/graph/application-rollkey-prooftoken) который можно использовать для создания этого доказательства маркера владения.</span><span class="sxs-lookup"><span data-stu-id="73a6c-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|


## <a name="response"></a><span data-ttu-id="73a6c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a6c-158">Response</span></span>

<span data-ttu-id="73a6c-159">В случае успешной работы этот метод возвращает код отклика и новый `200 OK` [объект keyCredential](../resources/keycredential.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73a6c-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73a6c-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="73a6c-160">Examples</span></span>

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a><span data-ttu-id="73a6c-161">Пример 1. Добавление новых учетных данных ключа в службуPrincipal</span><span class="sxs-lookup"><span data-stu-id="73a6c-161">Example 1: Adding a new key credential to a servicePrincipal</span></span>

#### <a name="request"></a><span data-ttu-id="73a6c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a6c-162">Request</span></span>

<span data-ttu-id="73a6c-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a6c-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73a6c-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="73a6c-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="73a6c-165">C#</span><span class="sxs-lookup"><span data-stu-id="73a6c-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73a6c-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73a6c-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73a6c-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73a6c-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73a6c-168">Java</span><span class="sxs-lookup"><span data-stu-id="73a6c-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73a6c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a6c-169">Response</span></span>

<span data-ttu-id="73a6c-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73a6c-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="73a6c-171">Пример 2. Добавление учетных данных ключа и связанного пароля для ключа</span><span class="sxs-lookup"><span data-stu-id="73a6c-171">Example 2: Adding a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="73a6c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a6c-172">Request</span></span>

<span data-ttu-id="73a6c-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a6c-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73a6c-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="73a6c-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="73a6c-175">C#</span><span class="sxs-lookup"><span data-stu-id="73a6c-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73a6c-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73a6c-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73a6c-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73a6c-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73a6c-178">Java</span><span class="sxs-lookup"><span data-stu-id="73a6c-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73a6c-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a6c-179">Response</span></span>

<span data-ttu-id="73a6c-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73a6c-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

