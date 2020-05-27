---
title: 'servicePrincipal: Аддкэй'
description: Добавление ключевых учетных данных в servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: be1e1cae6907b853a32cf0038f465127ea86f0b1
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383457"
---
# <a name="serviceprincipal-addkey"></a><span data-ttu-id="9097c-103">servicePrincipal: Аддкэй</span><span class="sxs-lookup"><span data-stu-id="9097c-103">servicePrincipal: addKey</span></span>

<span data-ttu-id="9097c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9097c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9097c-105">Добавление ключевых учетных данных в [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="9097c-105">Adds a key credential to a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="9097c-106">Этот метод вместе с [ремовекэй](serviceprincipal-removekey.md) можно использовать в servicePrincipal для автоматизации изкрутки ключей истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="9097c-106">This method along with [removeKey](serviceprincipal-removekey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="9097c-107">[Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [обновление операций servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления ключевых учетных данных для любых servicePrincipal с контекстом пользователя или без него.</span><span class="sxs-lookup"><span data-stu-id="9097c-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="9097c-108">В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия.</span><span class="sxs-lookup"><span data-stu-id="9097c-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="9097c-109">СервицепринЦипалс, у которых нет существующих действительных сертификатов (например, не было добавлено ни одного сертификата, или у всех сертификатов истек срок действия), не сможете использовать это действие службы.</span><span class="sxs-lookup"><span data-stu-id="9097c-109">ServicePrincipals that don’t have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="9097c-110">[Обновление servicePrincipal](../api/serviceprincipal-update.md) можно использовать для выполнения обновления.</span><span class="sxs-lookup"><span data-stu-id="9097c-110">[Update servicePrincipal](../api/serviceprincipal-update.md) can be used to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="9097c-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="9097c-111">Permissions</span></span>

|<span data-ttu-id="9097c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9097c-112">Permission type</span></span>      | <span data-ttu-id="9097c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9097c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9097c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9097c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9097c-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9097c-115">None.</span></span>  |
|<span data-ttu-id="9097c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9097c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9097c-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="9097c-117">None.</span></span>    |
|<span data-ttu-id="9097c-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="9097c-118">Application</span></span> | <span data-ttu-id="9097c-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9097c-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="9097c-120">ServicePrincipal не требует каких – либо специальных разрешений для развертывания собственных ключей.</span><span class="sxs-lookup"><span data-stu-id="9097c-120">A servicePrincipal does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="9097c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9097c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="9097c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9097c-122">Request headers</span></span>

| <span data-ttu-id="9097c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9097c-123">Name</span></span>           | <span data-ttu-id="9097c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9097c-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="9097c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9097c-125">Authorization</span></span>  | <span data-ttu-id="9097c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9097c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9097c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9097c-128">Content-Type</span></span>   | <span data-ttu-id="9097c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9097c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9097c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9097c-131">Request body</span></span>

<span data-ttu-id="9097c-132">В тексте запроса укажите следующие обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="9097c-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="9097c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="9097c-133">Property</span></span>     | <span data-ttu-id="9097c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9097c-134">Type</span></span>   |<span data-ttu-id="9097c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9097c-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9097c-136">кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="9097c-136">keyCredential</span></span> | [<span data-ttu-id="9097c-137">кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="9097c-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="9097c-138">Новые учетные данные ключа servicePrincipal для добавления.</span><span class="sxs-lookup"><span data-stu-id="9097c-138">The new servicePrincipal key credential to add.</span></span> <span data-ttu-id="9097c-139">Для этого использования требуются свойства __Type__, __Usage__ и __Key__ .</span><span class="sxs-lookup"><span data-stu-id="9097c-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="9097c-140">Поддерживаются следующие типы ключей:</span><span class="sxs-lookup"><span data-stu-id="9097c-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="9097c-141">`AsymmetricX509Cert`: Использование должно быть `Verify` .</span><span class="sxs-lookup"><span data-stu-id="9097c-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="9097c-142">`X509CertAndPassword`: Использование должно быть`Sign`</span><span class="sxs-lookup"><span data-stu-id="9097c-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="9097c-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="9097c-143">passwordCredential</span></span> | [<span data-ttu-id="9097c-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="9097c-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="9097c-145">Необходимо задать только __секреттекст__ , который должен содержать пароль для ключа.</span><span class="sxs-lookup"><span data-stu-id="9097c-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="9097c-146">Это свойство является обязательным только для ключей типа `X509CertAndPassword` .</span><span class="sxs-lookup"><span data-stu-id="9097c-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="9097c-147">Задайте для него значение `null` другой.</span><span class="sxs-lookup"><span data-stu-id="9097c-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="9097c-148">совмещен</span><span class="sxs-lookup"><span data-stu-id="9097c-148">proof</span></span> | <span data-ttu-id="9097c-149">String</span><span class="sxs-lookup"><span data-stu-id="9097c-149">String</span></span> | <span data-ttu-id="9097c-150">Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей.</span><span class="sxs-lookup"><span data-stu-id="9097c-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="9097c-151">Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="9097c-151">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="9097c-152">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="9097c-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="9097c-153">`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="9097c-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="9097c-154">`iss`-Issuer должен быть __идентификатором__ servicePrincipal, осуществляющим вызов.</span><span class="sxs-lookup"><span data-stu-id="9097c-154">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="9097c-155">`nbf`— Не до времени.</span><span class="sxs-lookup"><span data-stu-id="9097c-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="9097c-156">`exp`— Срок действия должен быть "NBF" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="9097c-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="9097c-157">Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9097c-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="9097c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9097c-158">Response</span></span>

<span data-ttu-id="9097c-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [кэйкредентиал](../resources/keycredential.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9097c-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9097c-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="9097c-160">Examples</span></span>

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a><span data-ttu-id="9097c-161">Пример 1: Добавление новых учетных данных ключа в объект servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="9097c-161">Example 1: Adding a new key credential to a servicePrincipal</span></span>

#### <a name="request"></a><span data-ttu-id="9097c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="9097c-162">Request</span></span>

<span data-ttu-id="9097c-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9097c-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9097c-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="9097c-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
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
# <a name="javascript"></a>[<span data-ttu-id="9097c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9097c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9097c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9097c-166">Response</span></span>

<span data-ttu-id="9097c-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9097c-167">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="9097c-168">Пример 2: Добавление учетных данных ключа и соответствующего пароля для ключа</span><span class="sxs-lookup"><span data-stu-id="9097c-168">Example 2: Adding a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="9097c-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="9097c-169">Request</span></span>

<span data-ttu-id="9097c-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9097c-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="9097c-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="9097c-171">Response</span></span>

<span data-ttu-id="9097c-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9097c-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
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
    "Error: serviceprincipal_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
