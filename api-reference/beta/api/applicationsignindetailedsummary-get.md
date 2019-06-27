---
title: Получение Аппликатионсигниндетаиледсуммари
description: Получение свойств и связей объекта Аппликатионсигниндетаилсуммари.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96b2e9bf87dd953ea6c53ae2d19c37c294425e35
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258403"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="aa1bc-103">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="aa1bc-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa1bc-104">Получение свойств и связей объекта [аппликатионсигниндетаилсуммари](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="aa1bc-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa1bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa1bc-105">Permissions</span></span>
<span data-ttu-id="aa1bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa1bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="aa1bc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa1bc-108">Permission type</span></span>                        | <span data-ttu-id="aa1bc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa1bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa1bc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa1bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa1bc-111">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="aa1bc-111">Report.Read.All</span></span> |
|<span data-ttu-id="aa1bc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa1bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa1bc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-113">Not supported.</span></span> |
|<span data-ttu-id="aa1bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa1bc-114">Application</span></span>                            | <span data-ttu-id="aa1bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa1bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa1bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa1bc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa1bc-117">Optional query parameters</span></span>

<span data-ttu-id="aa1bc-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa1bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa1bc-119">Request headers</span></span>

| <span data-ttu-id="aa1bc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aa1bc-120">Name</span></span>      |<span data-ttu-id="aa1bc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aa1bc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa1bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa1bc-122">Authorization</span></span> | <span data-ttu-id="aa1bc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aa1bc-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa1bc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa1bc-124">Request body</span></span>
<span data-ttu-id="aa1bc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa1bc-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa1bc-126">Response</span></span>
<span data-ttu-id="aa1bc-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аппликатионсигниндетаиледсуммари](../resources/applicationsignindetailedsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa1bc-128">Пример</span><span class="sxs-lookup"><span data-stu-id="aa1bc-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa1bc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa1bc-129">Request</span></span>
<span data-ttu-id="aa1bc-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```

### <a name="response"></a><span data-ttu-id="aa1bc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa1bc-131">Response</span></span>
<span data-ttu-id="aa1bc-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-132">The following is an example of the response.</span></span> 

><span data-ttu-id="aa1bc-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa1bc-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 295

{
  "id": "id-value",
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "status": {
    "errorCode": 99,
    "failureReason": "failureReason-value",
    "additionalDetails": "additionalDetails-value"
  },
  "signInCount": 99,
  "aggregatedEventDateTime": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aa1bc-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="aa1bc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aa1bc-136">C#</span><span class="sxs-lookup"><span data-stu-id="aa1bc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa1bc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa1bc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aa1bc-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aa1bc-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
