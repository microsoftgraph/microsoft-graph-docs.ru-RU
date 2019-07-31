---
title: Получение индикатора логики операций с угрозами
description: Получение свойств и связей объекта тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9fc33f36b33c1b12c4f183329a8bf03970b6c5c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977505"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="b4177-103">Получение индикатора логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="b4177-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4177-104">Получение свойств и связей объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="b4177-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4177-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4177-105">Permissions</span></span>

<span data-ttu-id="b4177-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4177-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4177-108">Permission type</span></span>                        | <span data-ttu-id="b4177-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4177-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4177-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4177-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4177-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b4177-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="b4177-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4177-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4177-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4177-113">Not supported.</span></span> |
| <span data-ttu-id="b4177-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4177-114">Application</span></span>                            | <span data-ttu-id="b4177-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b4177-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4177-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4177-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4177-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4177-117">Optional query parameters</span></span>

<span data-ttu-id="b4177-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4177-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b4177-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b4177-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4177-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4177-120">Request headers</span></span>

| <span data-ttu-id="b4177-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b4177-121">Name</span></span>      |<span data-ttu-id="b4177-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b4177-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4177-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4177-123">Authorization</span></span> | <span data-ttu-id="b4177-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b4177-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4177-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4177-125">Request body</span></span>

<span data-ttu-id="b4177-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4177-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4177-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4177-127">Response</span></span>

<span data-ttu-id="b4177-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4177-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4177-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4177-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4177-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4177-130">Request</span></span>

<span data-ttu-id="b4177-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4177-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4177-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4177-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4177-133">C#</span><span class="sxs-lookup"><span data-stu-id="b4177-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4177-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4177-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4177-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b4177-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4177-136">Java</span><span class="sxs-lookup"><span data-stu-id="b4177-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4177-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4177-137">Response</span></span>

<span data-ttu-id="b4177-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4177-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b4177-139">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b4177-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4177-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4177-140">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
