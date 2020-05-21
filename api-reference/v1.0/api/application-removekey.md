---
title: 'Приложение: Ремовекэй'
description: Удаление ключевых учетных данных из приложения
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a366da38cafd83c715f31f61ec01ecdcc6b7da1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334702"
---
# <a name="application-removekey"></a><span data-ttu-id="30631-103">Приложение: Ремовекэй</span><span class="sxs-lookup"><span data-stu-id="30631-103">application: removeKey</span></span>

<span data-ttu-id="30631-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30631-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30631-105">Удаление ключевых учетных данных из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="30631-105">Remove a key credential from an [application](../resources/application.md).</span></span> <span data-ttu-id="30631-106">Этот метод вместе с [аддкэй](application-addkey.md) может использоваться приложением для автоматизации пошаговых ключей истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="30631-106">This method along with [addKey](application-addkey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="30631-107">[Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [обновление операций servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления ключевых учетных данных для любого приложения с приложением или контекстом пользователя.</span><span class="sxs-lookup"><span data-stu-id="30631-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any application with application or a user's context.</span></span>

<span data-ttu-id="30631-108">В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия.</span><span class="sxs-lookup"><span data-stu-id="30631-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="30631-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="30631-109">Permissions</span></span>

|<span data-ttu-id="30631-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30631-110">Permission type</span></span>      | <span data-ttu-id="30631-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30631-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30631-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30631-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30631-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="30631-113">None.</span></span>  |
|<span data-ttu-id="30631-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30631-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30631-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="30631-115">None.</span></span>    |
|<span data-ttu-id="30631-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="30631-116">Application</span></span> | <span data-ttu-id="30631-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="30631-117">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="30631-118">Приложению не требуется определенное разрешение для развертывания собственных ключей.</span><span class="sxs-lookup"><span data-stu-id="30631-118">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="30631-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30631-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="30631-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30631-120">Request headers</span></span>

| <span data-ttu-id="30631-121">Имя</span><span class="sxs-lookup"><span data-stu-id="30631-121">Name</span></span>           | <span data-ttu-id="30631-122">Описание</span><span class="sxs-lookup"><span data-stu-id="30631-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="30631-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30631-123">Authorization</span></span>  | <span data-ttu-id="30631-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30631-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="30631-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30631-126">Content-Type</span></span>   | <span data-ttu-id="30631-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30631-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30631-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="30631-129">Request body</span></span>

<span data-ttu-id="30631-130">В тексте запроса укажите следующие обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="30631-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="30631-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="30631-131">Property</span></span>  | <span data-ttu-id="30631-132">Тип</span><span class="sxs-lookup"><span data-stu-id="30631-132">Type</span></span> | <span data-ttu-id="30631-133">Описание</span><span class="sxs-lookup"><span data-stu-id="30631-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="30631-134">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="30631-134">keyId</span></span>     | <span data-ttu-id="30631-135">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="30631-135">GUID</span></span> | <span data-ttu-id="30631-136">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="30631-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="30631-137">совмещен</span><span class="sxs-lookup"><span data-stu-id="30631-137">proof</span></span> | <span data-ttu-id="30631-138">String</span><span class="sxs-lookup"><span data-stu-id="30631-138">String</span></span> | <span data-ttu-id="30631-139">Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей.</span><span class="sxs-lookup"><span data-stu-id="30631-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="30631-140">Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов приложения.</span><span class="sxs-lookup"><span data-stu-id="30631-140">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="30631-141">Маркер должен содержать следующие утверждения:</span><span class="sxs-lookup"><span data-stu-id="30631-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="30631-142">`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="30631-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="30631-143">`iss`-Issuer должен быть __идентификатором__ приложения, осуществляющего вызов.</span><span class="sxs-lookup"><span data-stu-id="30631-143">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="30631-144">`nbf`— Не до времени.</span><span class="sxs-lookup"><span data-stu-id="30631-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="30631-145">`exp`— Срок действия должен быть "NBF" + 10 минут.</span><span class="sxs-lookup"><span data-stu-id="30631-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="30631-146">Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="30631-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="30631-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="30631-147">Response</span></span>

<span data-ttu-id="30631-148">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="30631-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="30631-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="30631-149">Examples</span></span>

<span data-ttu-id="30631-150">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="30631-150">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="30631-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="30631-151">Request</span></span>

<span data-ttu-id="30631-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30631-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="30631-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="30631-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="30631-154">C#</span><span class="sxs-lookup"><span data-stu-id="30631-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30631-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30631-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30631-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30631-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30631-157">Java</span><span class="sxs-lookup"><span data-stu-id="30631-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30631-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="30631-158">Response</span></span>

<span data-ttu-id="30631-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="30631-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
