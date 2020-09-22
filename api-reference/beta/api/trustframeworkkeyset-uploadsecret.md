---
title: 'Трустфрамеворккэйсет: Уплоадсекрет'
description: Отправьте секрет в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82d45f8af4e9a7a80626ad83c58b4fa58c5bb5de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095669"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="49a37-103">Трустфрамеворккэйсет: Уплоадсекрет</span><span class="sxs-lookup"><span data-stu-id="49a37-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="49a37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a37-105">Отправьте открытый текст секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="49a37-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="49a37-106">Примеры секретов — это секреты приложения в Azure Active Directory, Google, Facebook или любом другом поставщике удостоверений.</span><span class="sxs-lookup"><span data-stu-id="49a37-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="49a37-107">его метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="49a37-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49a37-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49a37-108">Permissions</span></span>

<span data-ttu-id="49a37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49a37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49a37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49a37-111">Permission type</span></span>                        | <span data-ttu-id="49a37-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49a37-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49a37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49a37-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="49a37-114">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="49a37-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="49a37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49a37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49a37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49a37-116">Not supported.</span></span> |
| <span data-ttu-id="49a37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49a37-117">Application</span></span>                            | <span data-ttu-id="49a37-118">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="49a37-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49a37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49a37-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="49a37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49a37-120">Request headers</span></span>

| <span data-ttu-id="49a37-121">Имя</span><span class="sxs-lookup"><span data-stu-id="49a37-121">Name</span></span>          | <span data-ttu-id="49a37-122">Описание</span><span class="sxs-lookup"><span data-stu-id="49a37-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49a37-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49a37-123">Authorization</span></span> | <span data-ttu-id="49a37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49a37-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49a37-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49a37-126">Content-type</span></span>  | <span data-ttu-id="49a37-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49a37-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49a37-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49a37-129">Request body</span></span>

<span data-ttu-id="49a37-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="49a37-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49a37-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="49a37-131">Parameter</span></span>    | <span data-ttu-id="49a37-132">Тип</span><span class="sxs-lookup"><span data-stu-id="49a37-132">Type</span></span>        | <span data-ttu-id="49a37-133">Описание</span><span class="sxs-lookup"><span data-stu-id="49a37-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49a37-134">Используйте</span><span class="sxs-lookup"><span data-stu-id="49a37-134">use</span></span>|<span data-ttu-id="49a37-135">Строка</span><span class="sxs-lookup"><span data-stu-id="49a37-135">String</span></span>|<span data-ttu-id="49a37-136">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="49a37-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="49a37-137">звонить</span><span class="sxs-lookup"><span data-stu-id="49a37-137">k</span></span>|<span data-ttu-id="49a37-138">Строка</span><span class="sxs-lookup"><span data-stu-id="49a37-138">String</span></span>|<span data-ttu-id="49a37-139">Аналогично свойству **k** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="49a37-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="49a37-140">Это поле, используемое для отправки секрета.</span><span class="sxs-lookup"><span data-stu-id="49a37-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="49a37-141">nbf</span><span class="sxs-lookup"><span data-stu-id="49a37-141">nbf</span></span>|<span data-ttu-id="49a37-142">Int64</span><span class="sxs-lookup"><span data-stu-id="49a37-142">Int64</span></span>|<span data-ttu-id="49a37-143">Аналогично свойству **NBF** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="49a37-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="49a37-144">exp</span><span class="sxs-lookup"><span data-stu-id="49a37-144">exp</span></span>|<span data-ttu-id="49a37-145">Int64</span><span class="sxs-lookup"><span data-stu-id="49a37-145">Int64</span></span>|<span data-ttu-id="49a37-146">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="49a37-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="49a37-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="49a37-147">Response</span></span>

<span data-ttu-id="49a37-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49a37-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49a37-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="49a37-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49a37-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="49a37-150">Request</span></span>

<span data-ttu-id="49a37-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49a37-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49a37-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="49a37-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```
# <a name="c"></a>[<span data-ttu-id="49a37-153">C#</span><span class="sxs-lookup"><span data-stu-id="49a37-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49a37-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49a37-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49a37-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49a37-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49a37-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="49a37-156">Response</span></span>

<span data-ttu-id="49a37-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49a37-157">The following is an example of the response.</span></span>

> <span data-ttu-id="49a37-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49a37-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


