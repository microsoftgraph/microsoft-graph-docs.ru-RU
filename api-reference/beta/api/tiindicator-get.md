---
title: Получение индикатора логики операций с угрозами
description: Получение свойств и связей объекта тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 23e6bf35f7e493b416be8ba4d4c2bab7df61e6d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270667"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="8785f-103">Получение индикатора логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="8785f-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8785f-104">Получение свойств и связей объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="8785f-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8785f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8785f-105">Permissions</span></span>

<span data-ttu-id="8785f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8785f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8785f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8785f-108">Permission type</span></span>                        | <span data-ttu-id="8785f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8785f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8785f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8785f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8785f-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="8785f-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="8785f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8785f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8785f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8785f-113">Not supported.</span></span> |
| <span data-ttu-id="8785f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8785f-114">Application</span></span>                            | <span data-ttu-id="8785f-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="8785f-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="8785f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8785f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8785f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8785f-117">Optional query parameters</span></span>

<span data-ttu-id="8785f-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8785f-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8785f-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8785f-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8785f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8785f-120">Request headers</span></span>

| <span data-ttu-id="8785f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8785f-121">Name</span></span>      |<span data-ttu-id="8785f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8785f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8785f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8785f-123">Authorization</span></span> | <span data-ttu-id="8785f-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8785f-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8785f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8785f-125">Request body</span></span>

<span data-ttu-id="8785f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8785f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8785f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8785f-127">Response</span></span>

<span data-ttu-id="8785f-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8785f-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8785f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8785f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8785f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8785f-130">Request</span></span>

<span data-ttu-id="8785f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8785f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="8785f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8785f-132">Response</span></span>

<span data-ttu-id="8785f-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8785f-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="8785f-134">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8785f-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8785f-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8785f-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8785f-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8785f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8785f-137">C#</span><span class="sxs-lookup"><span data-stu-id="8785f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8785f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8785f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tiindicator-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8785f-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8785f-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tiindicator-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
