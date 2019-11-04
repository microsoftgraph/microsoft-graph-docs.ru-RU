---
title: 'Трустфрамеворккэйсет: Уплоадсекрет'
description: Отправьте секрет в набор ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13742cee46164eaf2e21c4eefa2e8655fa4a567e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937493"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="06fbe-103">Трустфрамеворккэйсет: Уплоадсекрет</span><span class="sxs-lookup"><span data-stu-id="06fbe-103">trustFrameworkKeySet: uploadSecret</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06fbe-104">Отправьте открытый текст секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="06fbe-104">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="06fbe-105">Примеры секретов — это секреты приложения в Azure Active Directory, Google, Facebook или любом другом поставщике удостоверений.</span><span class="sxs-lookup"><span data-stu-id="06fbe-105">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="06fbe-106">его метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="06fbe-106">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06fbe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06fbe-107">Permissions</span></span>

<span data-ttu-id="06fbe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06fbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06fbe-110">Permission type</span></span>                        | <span data-ttu-id="06fbe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06fbe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06fbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06fbe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="06fbe-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06fbe-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="06fbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06fbe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06fbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06fbe-115">Not supported.</span></span> |
| <span data-ttu-id="06fbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06fbe-116">Application</span></span>                            | <span data-ttu-id="06fbe-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06fbe-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06fbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06fbe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="06fbe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06fbe-119">Request headers</span></span>

| <span data-ttu-id="06fbe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="06fbe-120">Name</span></span>          | <span data-ttu-id="06fbe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="06fbe-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="06fbe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06fbe-122">Authorization</span></span> | <span data-ttu-id="06fbe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fbe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06fbe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06fbe-125">Content-type</span></span>  | <span data-ttu-id="06fbe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fbe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06fbe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06fbe-128">Request body</span></span>

<span data-ttu-id="06fbe-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06fbe-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06fbe-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="06fbe-130">Parameter</span></span>    | <span data-ttu-id="06fbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06fbe-131">Type</span></span>        | <span data-ttu-id="06fbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06fbe-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06fbe-133">Используйте</span><span class="sxs-lookup"><span data-stu-id="06fbe-133">use</span></span>|<span data-ttu-id="06fbe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="06fbe-134">String</span></span>|<span data-ttu-id="06fbe-135">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="06fbe-135">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="06fbe-136">звонить</span><span class="sxs-lookup"><span data-stu-id="06fbe-136">k</span></span>|<span data-ttu-id="06fbe-137">Строка</span><span class="sxs-lookup"><span data-stu-id="06fbe-137">String</span></span>|<span data-ttu-id="06fbe-138">Аналогично свойству **k** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="06fbe-138">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="06fbe-139">Это поле, используемое для отправки секрета.</span><span class="sxs-lookup"><span data-stu-id="06fbe-139">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="06fbe-140">nbf</span><span class="sxs-lookup"><span data-stu-id="06fbe-140">nbf</span></span>|<span data-ttu-id="06fbe-141">Int64</span><span class="sxs-lookup"><span data-stu-id="06fbe-141">Int64</span></span>|<span data-ttu-id="06fbe-142">Аналогично свойству **NBF** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="06fbe-142">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="06fbe-143">exp</span><span class="sxs-lookup"><span data-stu-id="06fbe-143">exp</span></span>|<span data-ttu-id="06fbe-144">Int64</span><span class="sxs-lookup"><span data-stu-id="06fbe-144">Int64</span></span>|<span data-ttu-id="06fbe-145">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="06fbe-145">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="06fbe-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fbe-146">Response</span></span>

<span data-ttu-id="06fbe-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06fbe-147">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06fbe-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="06fbe-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06fbe-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="06fbe-149">Request</span></span>

<span data-ttu-id="06fbe-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06fbe-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06fbe-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="06fbe-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="06fbe-152">C#</span><span class="sxs-lookup"><span data-stu-id="06fbe-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06fbe-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06fbe-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06fbe-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06fbe-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06fbe-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fbe-155">Response</span></span>

<span data-ttu-id="06fbe-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06fbe-156">The following is an example of the response.</span></span>

> <span data-ttu-id="06fbe-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06fbe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
