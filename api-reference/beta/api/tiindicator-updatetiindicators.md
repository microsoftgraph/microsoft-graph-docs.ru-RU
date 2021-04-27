---
title: 'tiIndicator: updateTiIndicators'
description: Обновление нескольких индикаторов аналитики угроз (TI) в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4c594c9ba75ea0ee1cd1fcb8390d4b9ff738d48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050775"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="7d3ac-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="7d3ac-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="7d3ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d3ac-105">Обновление нескольких индикаторов аналитики угроз (TI) в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d3ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d3ac-106">Permissions</span></span>

<span data-ttu-id="7d3ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d3ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d3ac-109">Permission type</span></span>   | <span data-ttu-id="7d3ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d3ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7d3ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d3ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d3ac-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7d3ac-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="7d3ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d3ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d3ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-114">Not supported.</span></span> |
| <span data-ttu-id="7d3ac-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d3ac-115">Application</span></span>                            | <span data-ttu-id="7d3ac-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7d3ac-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d3ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d3ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="7d3ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d3ac-118">Request headers</span></span>

| <span data-ttu-id="7d3ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d3ac-119">Name</span></span>          | <span data-ttu-id="7d3ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d3ac-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7d3ac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d3ac-121">Authorization</span></span> | <span data-ttu-id="7d3ac-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7d3ac-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d3ac-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d3ac-123">Request body</span></span>

<span data-ttu-id="7d3ac-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="7d3ac-125">Сведения о свойствах, которые можно обновить, см. в обновленном [tiIndicator.](tiindicator-update.md)</span><span class="sxs-lookup"><span data-stu-id="7d3ac-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="7d3ac-126">Необходимые поля для каждого tiIndicator: `id` , `expirationDateTime` , `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="7d3ac-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="7d3ac-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d3ac-127">Parameter</span></span>    | <span data-ttu-id="7d3ac-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7d3ac-128">Type</span></span>        | <span data-ttu-id="7d3ac-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7d3ac-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d3ac-130">значение</span><span class="sxs-lookup"><span data-stu-id="7d3ac-130">value</span></span>|<span data-ttu-id="7d3ac-131">коллекция tiIndicator</span><span class="sxs-lookup"><span data-stu-id="7d3ac-131">tiIndicator collection</span></span>| <span data-ttu-id="7d3ac-132">Коллекция **tiIndicators** для обновления.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="7d3ac-133">Каждая сущность должна иметь **id** и другие редактируемые свойства для обновления.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="7d3ac-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3ac-134">Response</span></span>

<span data-ttu-id="7d3ac-135">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [tiIndicator](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="7d3ac-136">При ошибке этот метод возвращает `206 Partial Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="7d3ac-137">Дополнительные [сведения см. в](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) "Ошибках".</span><span class="sxs-lookup"><span data-stu-id="7d3ac-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="7d3ac-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d3ac-138">Examples</span></span>

<span data-ttu-id="7d3ac-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7d3ac-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d3ac-140">Request</span></span>

<span data-ttu-id="7d3ac-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d3ac-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d3ac-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="c"></a>[<span data-ttu-id="7d3ac-143">C#</span><span class="sxs-lookup"><span data-stu-id="7d3ac-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d3ac-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d3ac-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d3ac-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d3ac-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d3ac-146">Java</span><span class="sxs-lookup"><span data-stu-id="7d3ac-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7d3ac-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3ac-147">Response</span></span>

<span data-ttu-id="7d3ac-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7d3ac-149">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d3ac-149">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


