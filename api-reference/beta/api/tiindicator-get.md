---
title: Получение индикатора логики операций с угрозами
description: Получение свойств и связей объекта тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: fd5e6d027ecbb097406f280dfe02f9fe3c1a6c9b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977724"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="ff7f8-103">Получение индикатора логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="ff7f8-103">Get threat intelligence indicator</span></span>

<span data-ttu-id="ff7f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff7f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff7f8-105">Получение свойств и связей объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="ff7f8-105">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff7f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7f8-106">Permissions</span></span>

<span data-ttu-id="ff7f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff7f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff7f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7f8-109">Permission type</span></span>                        | <span data-ttu-id="ff7f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff7f8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff7f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff7f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff7f8-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ff7f8-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="ff7f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff7f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff7f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-114">Not supported.</span></span> |
| <span data-ttu-id="ff7f8-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ff7f8-115">Application</span></span>                            | <span data-ttu-id="ff7f8-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ff7f8-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff7f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff7f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff7f8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff7f8-118">Optional query parameters</span></span>

<span data-ttu-id="ff7f8-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff7f8-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff7f8-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff7f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff7f8-121">Request headers</span></span>

| <span data-ttu-id="ff7f8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ff7f8-122">Name</span></span>      |<span data-ttu-id="ff7f8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ff7f8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff7f8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff7f8-124">Authorization</span></span> | <span data-ttu-id="ff7f8-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff7f8-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff7f8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff7f8-126">Request body</span></span>

<span data-ttu-id="ff7f8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff7f8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff7f8-128">Response</span></span>

<span data-ttu-id="ff7f8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-129">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff7f8-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff7f8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff7f8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff7f8-131">Request</span></span>

<span data-ttu-id="ff7f8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff7f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff7f8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="ff7f8-134">C#</span><span class="sxs-lookup"><span data-stu-id="ff7f8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff7f8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff7f8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff7f8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff7f8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff7f8-137">Java</span><span class="sxs-lookup"><span data-stu-id="ff7f8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff7f8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff7f8-138">Response</span></span>

<span data-ttu-id="ff7f8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ff7f8-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff7f8-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff7f8-141">All the properties will be returned from an actual call.</span></span>

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


