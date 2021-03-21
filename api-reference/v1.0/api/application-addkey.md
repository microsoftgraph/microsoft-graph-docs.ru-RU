---
title: 'приложение: addKey'
description: Добавление учетных данных ключа в приложение.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2194af555769d8eb5423a5c08a59926cb3e004f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958789"
---
# <a name="application-addkey"></a><span data-ttu-id="fcce0-103">приложение: addKey</span><span class="sxs-lookup"><span data-stu-id="fcce0-103">application: addKey</span></span>

<span data-ttu-id="fcce0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcce0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcce0-105">Добавление учетных данных ключа в [приложение.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="fcce0-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="fcce0-106">Этот метод вместе с [removeKey](application-removekey.md) можно использовать приложением для автоматизации проката истекающих ключей.</span><span class="sxs-lookup"><span data-stu-id="fcce0-106">This method, along with [removeKey](application-removekey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="fcce0-107">[Создание операций](../api/application-post-applications.md) [приложения](../api/application-update.md) и обновления приложений можно продолжать использовать для добавления и обновления учетных данных для любого приложения с контекстом пользователя или без него.</span><span class="sxs-lookup"><span data-stu-id="fcce0-107">[Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) operations can continue to be used to add and update key credentials for any application with or without a user's context.</span></span>

<span data-ttu-id="fcce0-108">В рамках проверки запроса для этого метода проверяется доказательство на наличие существующего ключа перед выполнением действия.</span><span class="sxs-lookup"><span data-stu-id="fcce0-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="fcce0-109">Приложения, у которых нет существующих действительных сертификатов (еще не добавлены сертификаты или истек срок действия всех сертификатов), не смогут использовать это действие службы.</span><span class="sxs-lookup"><span data-stu-id="fcce0-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="fcce0-110">Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](../api/application-update.md).</span><span class="sxs-lookup"><span data-stu-id="fcce0-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcce0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcce0-111">Permissions</span></span>

|<span data-ttu-id="fcce0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcce0-112">Permission type</span></span>      | <span data-ttu-id="fcce0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcce0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcce0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcce0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fcce0-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fcce0-115">None.</span></span>  |
|<span data-ttu-id="fcce0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcce0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcce0-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="fcce0-117">None.</span></span>    |
|<span data-ttu-id="fcce0-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcce0-118">Application</span></span> | <span data-ttu-id="fcce0-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fcce0-119">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="fcce0-120">Приложение не нуждается в специальном разрешении для сверки собственных ключей.</span><span class="sxs-lookup"><span data-stu-id="fcce0-120">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="fcce0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcce0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="fcce0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcce0-122">Request headers</span></span>

| <span data-ttu-id="fcce0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fcce0-123">Name</span></span>           | <span data-ttu-id="fcce0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fcce0-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fcce0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcce0-125">Authorization</span></span>  | <span data-ttu-id="fcce0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcce0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fcce0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcce0-128">Content-Type</span></span>   | <span data-ttu-id="fcce0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcce0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcce0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcce0-131">Request body</span></span>

<span data-ttu-id="fcce0-132">В теле запроса укажи следующие необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="fcce0-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="fcce0-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcce0-133">Property</span></span>     | <span data-ttu-id="fcce0-134">Тип</span><span class="sxs-lookup"><span data-stu-id="fcce0-134">Type</span></span>   |<span data-ttu-id="fcce0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="fcce0-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fcce0-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="fcce0-136">keyCredential</span></span> | [<span data-ttu-id="fcce0-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="fcce0-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="fcce0-138">Добавлены новые учетные данные ключа приложения.</span><span class="sxs-lookup"><span data-stu-id="fcce0-138">The new application key credential to add.</span></span> <span data-ttu-id="fcce0-139">__Тип,__ __использование и__ __ключ__ необходимые свойства для этого использования.</span><span class="sxs-lookup"><span data-stu-id="fcce0-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="fcce0-140">Поддерживаемые ключевые типы:</span><span class="sxs-lookup"><span data-stu-id="fcce0-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="fcce0-141">`AsymmetricX509Cert`: Использование должно быть `Verify` .</span><span class="sxs-lookup"><span data-stu-id="fcce0-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="fcce0-142">`X509CertAndPassword`: Использование должно быть `Sign`</span><span class="sxs-lookup"><span data-stu-id="fcce0-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="fcce0-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="fcce0-143">passwordCredential</span></span> | [<span data-ttu-id="fcce0-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="fcce0-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="fcce0-145">Требуется __установить только secretText,__ который должен содержать пароль для ключа.</span><span class="sxs-lookup"><span data-stu-id="fcce0-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="fcce0-146">Это свойство требуется только для ключей типа `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="fcce0-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="fcce0-147">Установите его в `null` противном случае.</span><span class="sxs-lookup"><span data-stu-id="fcce0-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="fcce0-148">доказательство</span><span class="sxs-lookup"><span data-stu-id="fcce0-148">proof</span></span> | <span data-ttu-id="fcce0-149">String</span><span class="sxs-lookup"><span data-stu-id="fcce0-149">String</span></span> | <span data-ttu-id="fcce0-150">Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами.</span><span class="sxs-lookup"><span data-stu-id="fcce0-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="fcce0-151">Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения.</span><span class="sxs-lookup"><span data-stu-id="fcce0-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="fcce0-152">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="fcce0-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="fcce0-153">`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="fcce0-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="fcce0-154">`iss` — издателем должен быть __идентификатор__  приложения, выполняющего вызов.</span><span class="sxs-lookup"><span data-stu-id="fcce0-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="fcce0-155">`nbf` — вовремя.</span><span class="sxs-lookup"><span data-stu-id="fcce0-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="fcce0-156">`exp` — сроком действия должно быть значение "nbf" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="fcce0-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="fcce0-157">Вот пример [кода,](/graph/application-rollkey-prooftoken) который можно использовать для создания этого доказательства маркера владения.</span><span class="sxs-lookup"><span data-stu-id="fcce0-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="fcce0-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcce0-158">Response</span></span>

<span data-ttu-id="fcce0-159">В случае успешной работы этот метод возвращает код отклика и новый `200 OK` [объект keyCredential](../resources/keycredential.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcce0-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fcce0-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="fcce0-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="fcce0-161">Пример 1. Добавление новых учетных данных ключей в приложение</span><span class="sxs-lookup"><span data-stu-id="fcce0-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="fcce0-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcce0-162">Request</span></span>

<span data-ttu-id="fcce0-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcce0-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcce0-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcce0-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
# <a name="c"></a>[<span data-ttu-id="fcce0-165">C#</span><span class="sxs-lookup"><span data-stu-id="fcce0-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcce0-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcce0-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcce0-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcce0-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcce0-168">Java</span><span class="sxs-lookup"><span data-stu-id="fcce0-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fcce0-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcce0-169">Response</span></span>

<span data-ttu-id="fcce0-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcce0-170">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="fcce0-171">Пример 2. Добавление учетных данных ключа и связанного пароля для ключа</span><span class="sxs-lookup"><span data-stu-id="fcce0-171">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="fcce0-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcce0-172">Request</span></span>

<span data-ttu-id="fcce0-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcce0-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcce0-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcce0-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
# <a name="c"></a>[<span data-ttu-id="fcce0-175">C#</span><span class="sxs-lookup"><span data-stu-id="fcce0-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcce0-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcce0-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcce0-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcce0-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcce0-178">Java</span><span class="sxs-lookup"><span data-stu-id="fcce0-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fcce0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcce0-179">Response</span></span>

<span data-ttu-id="fcce0-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fcce0-180">The following is an example of the response.</span></span>

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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

