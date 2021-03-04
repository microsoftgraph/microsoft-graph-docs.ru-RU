---
title: 'trustFrameworkKeySet: uploadSecret'
description: Загрузите секрет в набор ключей.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b008e1ae41d61fb14dbd80e5a820208355bb670d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444975"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="a4f02-103">trustFrameworkKeySet: uploadSecret</span><span class="sxs-lookup"><span data-stu-id="a4f02-103">trustFrameworkKeySet: uploadSecret</span></span>

<span data-ttu-id="a4f02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f02-105">Загрузите простой текстовый секрет в [trustFrameworkKeyset.](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="a4f02-105">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="a4f02-106">Примеры секретов — секреты приложений в Azure Active Directory, Google, Facebook или любом другом поставщике удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a4f02-106">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="a4f02-107">его метод возвращает [trustFrameworkKey](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="a4f02-107">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f02-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f02-108">Permissions</span></span>

<span data-ttu-id="a4f02-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4f02-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f02-111">Permission type</span></span>                        | <span data-ttu-id="a4f02-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4f02-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a4f02-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f02-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4f02-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f02-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="a4f02-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f02-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4f02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f02-116">Not supported.</span></span> |
| <span data-ttu-id="a4f02-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4f02-117">Application</span></span>                            | <span data-ttu-id="a4f02-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f02-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4f02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f02-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="a4f02-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4f02-120">Request headers</span></span>

| <span data-ttu-id="a4f02-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a4f02-121">Name</span></span>          | <span data-ttu-id="a4f02-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f02-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a4f02-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f02-123">Authorization</span></span> | <span data-ttu-id="a4f02-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f02-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4f02-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4f02-126">Content-type</span></span>  | <span data-ttu-id="a4f02-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f02-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4f02-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4f02-129">Request body</span></span>

<span data-ttu-id="a4f02-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a4f02-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4f02-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="a4f02-131">Parameter</span></span>    | <span data-ttu-id="a4f02-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f02-132">Type</span></span>        | <span data-ttu-id="a4f02-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f02-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4f02-134">использование</span><span class="sxs-lookup"><span data-stu-id="a4f02-134">use</span></span>|<span data-ttu-id="a4f02-135">String</span><span class="sxs-lookup"><span data-stu-id="a4f02-135">String</span></span>|<span data-ttu-id="a4f02-136">Аналогично **свойству использования** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="a4f02-136">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="a4f02-137">k</span><span class="sxs-lookup"><span data-stu-id="a4f02-137">k</span></span>|<span data-ttu-id="a4f02-138">String</span><span class="sxs-lookup"><span data-stu-id="a4f02-138">String</span></span>|<span data-ttu-id="a4f02-139">Аналогично свойству **k** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="a4f02-139">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="a4f02-140">Это поле, которое используется для отправки секрета.</span><span class="sxs-lookup"><span data-stu-id="a4f02-140">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="a4f02-141">nbf</span><span class="sxs-lookup"><span data-stu-id="a4f02-141">nbf</span></span>|<span data-ttu-id="a4f02-142">Int64</span><span class="sxs-lookup"><span data-stu-id="a4f02-142">Int64</span></span>|<span data-ttu-id="a4f02-143">Аналогично свойству **nbf** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="a4f02-143">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="a4f02-144">exp</span><span class="sxs-lookup"><span data-stu-id="a4f02-144">exp</span></span>|<span data-ttu-id="a4f02-145">Int64</span><span class="sxs-lookup"><span data-stu-id="a4f02-145">Int64</span></span>|<span data-ttu-id="a4f02-146">Аналогично свойству **exp** **trustFrameworkKey.**</span><span class="sxs-lookup"><span data-stu-id="a4f02-146">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="a4f02-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f02-147">Response</span></span>

<span data-ttu-id="a4f02-148">В случае успеха этот метод возвращает код отклика и новый `200 OK` [объект trustFrameworkKey](../resources/trustframeworkkey.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4f02-148">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4f02-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4f02-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4f02-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f02-150">Request</span></span>

<span data-ttu-id="a4f02-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4f02-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4f02-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f02-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a4f02-153">C#</span><span class="sxs-lookup"><span data-stu-id="a4f02-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4f02-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4f02-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4f02-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4f02-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4f02-156">Java</span><span class="sxs-lookup"><span data-stu-id="a4f02-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadsecret-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4f02-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f02-157">Response</span></span>

<span data-ttu-id="a4f02-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4f02-158">The following is an example of the response.</span></span>

> <span data-ttu-id="a4f02-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4f02-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


