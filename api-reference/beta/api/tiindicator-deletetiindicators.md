---
title: 'Тииндикатор: Делететииндикаторс'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9e11defaf3d505d5566c9d5d720e26b6c88447a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022213"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="1938e-103">Тииндикатор: Делететииндикаторс</span><span class="sxs-lookup"><span data-stu-id="1938e-103">tiIndicator: deleteTiIndicators</span></span>

<span data-ttu-id="1938e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1938e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1938e-105">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.</span><span class="sxs-lookup"><span data-stu-id="1938e-105">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="1938e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1938e-106">Permissions</span></span>

<span data-ttu-id="1938e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1938e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1938e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1938e-109">Permission type</span></span> | <span data-ttu-id="1938e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1938e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1938e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1938e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1938e-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1938e-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="1938e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1938e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1938e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1938e-114">Not supported.</span></span> |
| <span data-ttu-id="1938e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1938e-115">Application</span></span>                            | <span data-ttu-id="1938e-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1938e-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1938e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1938e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="1938e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1938e-118">Request headers</span></span>

| <span data-ttu-id="1938e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1938e-119">Name</span></span>          | <span data-ttu-id="1938e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1938e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1938e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1938e-121">Authorization</span></span> | <span data-ttu-id="1938e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1938e-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1938e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1938e-123">Request body</span></span>

<span data-ttu-id="1938e-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1938e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1938e-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="1938e-125">Parameter</span></span>    | <span data-ttu-id="1938e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1938e-126">Type</span></span>        | <span data-ttu-id="1938e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1938e-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1938e-128">значение</span><span class="sxs-lookup"><span data-stu-id="1938e-128">value</span></span>|<span data-ttu-id="1938e-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1938e-129">String collection</span></span>| <span data-ttu-id="1938e-130">Коллекция Тииндикатор `id` s, которую необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="1938e-130">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="1938e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1938e-131">Response</span></span>

<span data-ttu-id="1938e-132">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1938e-132">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="1938e-133">При возникновении ошибки этот метод возвращает `206 Partial Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="1938e-133">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="1938e-134">Дополнительные сведения см. в разделе [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) .</span><span class="sxs-lookup"><span data-stu-id="1938e-134">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="1938e-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="1938e-135">Examples</span></span>

<span data-ttu-id="1938e-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1938e-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1938e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1938e-137">Request</span></span>

<span data-ttu-id="1938e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1938e-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1938e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1938e-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1938e-140">C#</span><span class="sxs-lookup"><span data-stu-id="1938e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1938e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1938e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1938e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1938e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1938e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1938e-143">Response</span></span>

<span data-ttu-id="1938e-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1938e-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1938e-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1938e-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1938e-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1938e-146">All the properties will be returned from an actual call.</span></span>

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


