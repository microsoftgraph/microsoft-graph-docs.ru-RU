---
title: 'Тииндикатор: Делететииндикаторсбекстерналид'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов, а запрос содержит внешние идентификаторы, а не идентификаторы.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 04d9e95bce724f354c7e1a39e49083dd3cc3c090
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042823"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="e2b39-103">Тииндикатор: Делететииндикаторсбекстерналид</span><span class="sxs-lookup"><span data-stu-id="e2b39-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

<span data-ttu-id="e2b39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2b39-105">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе вместо нескольких запросов, если запрос содержит внешние идентификаторы, а не идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="e2b39-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2b39-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2b39-106">Permissions</span></span>

<span data-ttu-id="e2b39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2b39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2b39-109">Permission type</span></span>  | <span data-ttu-id="e2b39-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2b39-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2b39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2b39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2b39-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e2b39-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e2b39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2b39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2b39-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2b39-114">Not supported.</span></span> |
| <span data-ttu-id="e2b39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2b39-115">Application</span></span>                            | <span data-ttu-id="e2b39-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e2b39-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2b39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2b39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="e2b39-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2b39-118">Request headers</span></span>

| <span data-ttu-id="e2b39-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2b39-119">Name</span></span>          | <span data-ttu-id="e2b39-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2b39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e2b39-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2b39-121">Authorization</span></span> | <span data-ttu-id="e2b39-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e2b39-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2b39-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2b39-123">Request body</span></span>

<span data-ttu-id="e2b39-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e2b39-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2b39-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2b39-125">Parameter</span></span>    | <span data-ttu-id="e2b39-126">Тип</span><span class="sxs-lookup"><span data-stu-id="e2b39-126">Type</span></span>        | <span data-ttu-id="e2b39-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e2b39-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2b39-128">значение</span><span class="sxs-lookup"><span data-stu-id="e2b39-128">value</span></span>|<span data-ttu-id="e2b39-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2b39-129">String collection</span></span>| <span data-ttu-id="e2b39-130">Коллекция `externalIds` объектов **тииндикатор** , которые необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="e2b39-130">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="e2b39-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2b39-131">Response</span></span>

<span data-ttu-id="e2b39-132">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2b39-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="e2b39-133">При возникновении ошибки этот метод возвращает `206 Partial Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="e2b39-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="e2b39-134">Дополнительные сведения см. в разделе [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) .</span><span class="sxs-lookup"><span data-stu-id="e2b39-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="e2b39-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="e2b39-135">Examples</span></span>

<span data-ttu-id="e2b39-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e2b39-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e2b39-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2b39-137">Request</span></span>

<span data-ttu-id="e2b39-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2b39-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2b39-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b39-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="e2b39-140">C#</span><span class="sxs-lookup"><span data-stu-id="e2b39-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2b39-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2b39-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2b39-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2b39-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2b39-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2b39-143">Response</span></span>

<span data-ttu-id="e2b39-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e2b39-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e2b39-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e2b39-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2b39-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2b39-146">All the properties will be returned from an actual call.</span></span>

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
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


