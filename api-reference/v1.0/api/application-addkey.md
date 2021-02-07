---
title: 'application: addKey'
description: Добавление учетных данных ключа в приложение.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c6beab8c5c5caff07778765e13e1836944238a4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131872"
---
# <a name="application-addkey"></a><span data-ttu-id="4f6dd-103">application: addKey</span><span class="sxs-lookup"><span data-stu-id="4f6dd-103">application: addKey</span></span>

<span data-ttu-id="4f6dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f6dd-105">Добавьте учетные данные ключа в [приложение.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="4f6dd-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="4f6dd-106">Этот метод, а также [removeKey](application-removekey.md) может использоваться приложением для автоматизации перетаскивания ключей окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-106">This method, along with [removeKey](application-removekey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="4f6dd-107">[Операции](../api/application-post-applications.md) создания [приложений](../api/application-update.md) и обновления приложений можно продолжать использовать для добавления и обновления учетных данных ключей для любого приложения с контекстом пользователя или без него.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-107">[Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) operations can continue to be used to add and update key credentials for any application with or without a user's context.</span></span>

<span data-ttu-id="4f6dd-108">В рамках проверки запроса для этого метода перед выполнением действия проверяется подтверждение на владение существующим ключом.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="4f6dd-109">Приложения, у которых нет действительных сертификатов (сертификаты еще не добавлены или срок действия всех сертификатов истек), не смогут использовать это действие службы.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="4f6dd-110">Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](../api/application-update.md).</span><span class="sxs-lookup"><span data-stu-id="4f6dd-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f6dd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6dd-111">Permissions</span></span>

|<span data-ttu-id="4f6dd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6dd-112">Permission type</span></span>      | <span data-ttu-id="4f6dd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6dd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f6dd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6dd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f6dd-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-115">None.</span></span>  |
|<span data-ttu-id="4f6dd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6dd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6dd-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-117">None.</span></span>    |
|<span data-ttu-id="4f6dd-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f6dd-118">Application</span></span> | <span data-ttu-id="4f6dd-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-119">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="4f6dd-120">Приложению не требуется никаких специальных разрешений для переката собственных ключей.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-120">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f6dd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6dd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="4f6dd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f6dd-122">Request headers</span></span>

| <span data-ttu-id="4f6dd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4f6dd-123">Name</span></span>           | <span data-ttu-id="4f6dd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6dd-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4f6dd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f6dd-125">Authorization</span></span>  | <span data-ttu-id="4f6dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4f6dd-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f6dd-128">Content-Type</span></span>   | <span data-ttu-id="4f6dd-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6dd-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f6dd-131">Request body</span></span>

<span data-ttu-id="4f6dd-132">В теле запроса укажив следующие необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="4f6dd-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f6dd-133">Property</span></span>     | <span data-ttu-id="4f6dd-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6dd-134">Type</span></span>   |<span data-ttu-id="4f6dd-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6dd-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f6dd-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="4f6dd-136">keyCredential</span></span> | [<span data-ttu-id="4f6dd-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="4f6dd-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="4f6dd-138">Новые учетные данные ключа приложения, которые необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-138">The new application key credential to add.</span></span> <span data-ttu-id="4f6dd-139">Свойства __типа,__ __использования__ __и ключа__ являются обязательной для этого использования.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="4f6dd-140">Поддерживаемые типы ключей:</span><span class="sxs-lookup"><span data-stu-id="4f6dd-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="4f6dd-141">`AsymmetricX509Cert`: использование должно быть `Verify` .</span><span class="sxs-lookup"><span data-stu-id="4f6dd-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="4f6dd-142">`X509CertAndPassword`: использование должно быть `Sign`</span><span class="sxs-lookup"><span data-stu-id="4f6dd-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="4f6dd-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="4f6dd-143">passwordCredential</span></span> | [<span data-ttu-id="4f6dd-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="4f6dd-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="4f6dd-145">Требуется __установить только secretText,__ который должен содержать пароль для ключа.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="4f6dd-146">Это свойство требуется только для ключей `X509CertAndPassword` типа.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="4f6dd-147">В противном `null` случае.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="4f6dd-148">proof</span><span class="sxs-lookup"><span data-stu-id="4f6dd-148">proof</span></span> | <span data-ttu-id="4f6dd-149">String</span><span class="sxs-lookup"><span data-stu-id="4f6dd-149">String</span></span> | <span data-ttu-id="4f6dd-150">Самозаверяющая маркер JWT, используемая в качестве подтверждения владения существующими ключами.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="4f6dd-151">Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="4f6dd-152">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="4f6dd-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="4f6dd-153">`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="4f6dd-154">`iss` — издателем должен быть __идентификатор__  приложения, выполняющего вызов.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="4f6dd-155">`nbf` — вовремя.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="4f6dd-156">`exp` — сроком действия должно быть значение "nbf" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="4f6dd-157">Вот пример [кода, который](/graph/application-rollkey-prooftoken) можно использовать для создания этого подтверждения маркера владения.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="4f6dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6dd-158">Response</span></span>

<span data-ttu-id="4f6dd-159">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект keyCredential](../resources/keycredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f6dd-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f6dd-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="4f6dd-161">Пример 1. Добавление новых учетных данных ключа в приложение</span><span class="sxs-lookup"><span data-stu-id="4f6dd-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="4f6dd-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6dd-162">Request</span></span>

<span data-ttu-id="4f6dd-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4f6dd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6dd-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
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
# <a name="c"></a>[<span data-ttu-id="4f6dd-165">C#</span><span class="sxs-lookup"><span data-stu-id="4f6dd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6dd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6dd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6dd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6dd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6dd-168">Java</span><span class="sxs-lookup"><span data-stu-id="4f6dd-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4f6dd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6dd-169">Response</span></span>

<span data-ttu-id="4f6dd-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-170">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="4f6dd-171">Пример 2. Добавление учетных данных ключа и связанного пароля для ключа</span><span class="sxs-lookup"><span data-stu-id="4f6dd-171">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="4f6dd-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6dd-172">Request</span></span>

<span data-ttu-id="4f6dd-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
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

#### <a name="response"></a><span data-ttu-id="4f6dd-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6dd-174">Response</span></span>

<span data-ttu-id="4f6dd-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f6dd-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
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
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->

