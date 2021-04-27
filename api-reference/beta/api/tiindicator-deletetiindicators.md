---
title: 'tiIndicator: deleteTiIndicators'
description: Удалите несколько индикаторов разведки угроз (TI) в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 365f4c803cb7f6e7b18570534819e576990d11de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050796"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="4bbc1-103">tiIndicator: deleteTiIndicators</span><span class="sxs-lookup"><span data-stu-id="4bbc1-103">tiIndicator: deleteTiIndicators</span></span>

<span data-ttu-id="4bbc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bbc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bbc1-105">Удалите несколько индикаторов разведки угроз (TI) в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bbc1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bbc1-106">Permissions</span></span>

<span data-ttu-id="4bbc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bbc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bbc1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bbc1-109">Permission type</span></span> | <span data-ttu-id="4bbc1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bbc1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bbc1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bbc1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bbc1-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4bbc1-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="4bbc1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bbc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bbc1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-114">Not supported.</span></span> |
| <span data-ttu-id="4bbc1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4bbc1-115">Application</span></span>                            | <span data-ttu-id="4bbc1-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4bbc1-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bbc1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bbc1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="4bbc1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bbc1-118">Request headers</span></span>

| <span data-ttu-id="4bbc1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4bbc1-119">Name</span></span>          | <span data-ttu-id="4bbc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4bbc1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4bbc1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bbc1-121">Authorization</span></span> | <span data-ttu-id="4bbc1-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4bbc1-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bbc1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bbc1-123">Request body</span></span>

<span data-ttu-id="4bbc1-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bbc1-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4bbc1-125">Parameter</span></span>    | <span data-ttu-id="4bbc1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4bbc1-126">Type</span></span>        | <span data-ttu-id="4bbc1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4bbc1-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4bbc1-128">значение</span><span class="sxs-lookup"><span data-stu-id="4bbc1-128">value</span></span>|<span data-ttu-id="4bbc1-129">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4bbc1-129">String collection</span></span>| <span data-ttu-id="4bbc1-130">Коллекция tiIndicator `id` s, которая будет удалена.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-130">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="4bbc1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bbc1-131">Response</span></span>

<span data-ttu-id="4bbc1-132">В случае успешной работы этот метод возвращает код ответа и `200, OK` [объект коллекции resultInfo](../resources/resultinfo.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="4bbc1-133">При ошибке этот метод возвращает `206 Partial Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="4bbc1-134">Дополнительные [сведения см. в](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) "Ошибках".</span><span class="sxs-lookup"><span data-stu-id="4bbc1-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="4bbc1-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="4bbc1-135">Examples</span></span>

<span data-ttu-id="4bbc1-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4bbc1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bbc1-137">Request</span></span>

<span data-ttu-id="4bbc1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bbc1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bbc1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="4bbc1-140">C#</span><span class="sxs-lookup"><span data-stu-id="4bbc1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bbc1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bbc1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bbc1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bbc1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bbc1-143">Java</span><span class="sxs-lookup"><span data-stu-id="4bbc1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-deletetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4bbc1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bbc1-144">Response</span></span>

<span data-ttu-id="4bbc1-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4bbc1-146">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4bbc1-146">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": 0,
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


