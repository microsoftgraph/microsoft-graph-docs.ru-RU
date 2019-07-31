---
title: Список индикаторов логики операций с угрозами
description: Получение списка объектов тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4e4aa089614548379dc23e92bec5fff50696fc5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987917"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="e8f6b-103">Список индикаторов логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="e8f6b-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8f6b-104">Получение списка объектов [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f6b-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8f6b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8f6b-105">Permissions</span></span>

<span data-ttu-id="e8f6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8f6b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8f6b-108">Permission type</span></span>     | <span data-ttu-id="e8f6b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8f6b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8f6b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8f6b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8f6b-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8f6b-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="e8f6b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8f6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8f6b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-113">Not supported.</span></span> |
| <span data-ttu-id="e8f6b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8f6b-114">Application</span></span>                            | <span data-ttu-id="e8f6b-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e8f6b-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8f6b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8f6b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8f6b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8f6b-117">Optional query parameters</span></span>

<span data-ttu-id="e8f6b-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8f6b-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8f6b-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8f6b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8f6b-120">Request headers</span></span>

| <span data-ttu-id="e8f6b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e8f6b-121">Name</span></span>      |<span data-ttu-id="e8f6b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e8f6b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8f6b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8f6b-123">Authorization</span></span> | <span data-ttu-id="e8f6b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e8f6b-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8f6b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8f6b-125">Request body</span></span>

<span data-ttu-id="e8f6b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8f6b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f6b-127">Response</span></span>

<span data-ttu-id="e8f6b-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8f6b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8f6b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8f6b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8f6b-130">Request</span></span>

<span data-ttu-id="e8f6b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8f6b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8f6b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8f6b-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8f6b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8f6b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8f6b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8f6b-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e8f6b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8f6b-136">Java</span><span class="sxs-lookup"><span data-stu-id="e8f6b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8f6b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f6b-137">Response</span></span>

<span data-ttu-id="e8f6b-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e8f6b-139">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8f6b-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8f6b-140">All the properties will be returned from an actual call.</span></span>

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
