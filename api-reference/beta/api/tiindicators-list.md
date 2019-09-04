---
title: Список индикаторов логики операций с угрозами
description: Получение списка объектов тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a16728c1f6c1685dbe2584580475a1169d9dd96e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722148"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="b81a5-103">Список индикаторов логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="b81a5-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b81a5-104">Получение списка объектов [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="b81a5-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b81a5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b81a5-105">Permissions</span></span>

<span data-ttu-id="b81a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b81a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b81a5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b81a5-108">Permission type</span></span>     | <span data-ttu-id="b81a5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b81a5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b81a5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b81a5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b81a5-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b81a5-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="b81a5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b81a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b81a5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b81a5-113">Not supported.</span></span> |
| <span data-ttu-id="b81a5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b81a5-114">Application</span></span>                            | <span data-ttu-id="b81a5-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b81a5-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="b81a5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b81a5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b81a5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b81a5-117">Optional query parameters</span></span>

<span data-ttu-id="b81a5-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b81a5-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b81a5-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b81a5-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b81a5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b81a5-120">Request headers</span></span>

| <span data-ttu-id="b81a5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b81a5-121">Name</span></span>      |<span data-ttu-id="b81a5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b81a5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b81a5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b81a5-123">Authorization</span></span> | <span data-ttu-id="b81a5-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b81a5-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b81a5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b81a5-125">Request body</span></span>

<span data-ttu-id="b81a5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b81a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b81a5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b81a5-127">Response</span></span>

<span data-ttu-id="b81a5-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b81a5-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b81a5-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b81a5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b81a5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b81a5-130">Request</span></span>

<span data-ttu-id="b81a5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b81a5-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b81a5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b81a5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b81a5-133">C#</span><span class="sxs-lookup"><span data-stu-id="b81a5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b81a5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b81a5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b81a5-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b81a5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b81a5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b81a5-136">Response</span></span>

<span data-ttu-id="b81a5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b81a5-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b81a5-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b81a5-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b81a5-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b81a5-139">All the properties will be returned from an actual call.</span></span>

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
      "action": "action-value",
      "activityGroupNames": [
        "activityGroupNames-value"
      ],
      "additionalInformation": "additionalInformation-value",
      "azureTenantId": "azureTenantId-value",
      "confidence": 99,
      "description": "description-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
