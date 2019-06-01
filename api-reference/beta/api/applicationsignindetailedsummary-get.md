---
title: Получение Аппликатионсигниндетаиледсуммари
description: Получение свойств и связей объекта Аппликатионсигниндетаилсуммари.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2145bfb511c1460b8001aa9eee9c1087fec460ba
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655105"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="5cbd5-103">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="5cbd5-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cbd5-104">Получение свойств и связей объекта [аппликатионсигниндетаилсуммари](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5cbd5-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cbd5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cbd5-105">Permissions</span></span>
<span data-ttu-id="5cbd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cbd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="5cbd5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cbd5-108">Permission type</span></span>                        | <span data-ttu-id="5cbd5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cbd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cbd5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cbd5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cbd5-111">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5cbd5-111">Report.Read.All</span></span> |
|<span data-ttu-id="5cbd5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cbd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cbd5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-113">Not supported.</span></span> |
|<span data-ttu-id="5cbd5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cbd5-114">Application</span></span>                            | <span data-ttu-id="5cbd5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cbd5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cbd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cbd5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cbd5-117">Optional query parameters</span></span>

<span data-ttu-id="5cbd5-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cbd5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cbd5-119">Request headers</span></span>

| <span data-ttu-id="5cbd5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5cbd5-120">Name</span></span>      |<span data-ttu-id="5cbd5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5cbd5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5cbd5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cbd5-122">Authorization</span></span> | <span data-ttu-id="5cbd5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5cbd5-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cbd5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cbd5-124">Request body</span></span>
<span data-ttu-id="5cbd5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cbd5-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cbd5-126">Response</span></span>
<span data-ttu-id="5cbd5-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аппликатионсигниндетаиледсуммари](../resources/applicationsignindetailedsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cbd5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5cbd5-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cbd5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cbd5-129">Request</span></span>
<span data-ttu-id="5cbd5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```

### <a name="response"></a><span data-ttu-id="5cbd5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cbd5-131">Response</span></span>
<span data-ttu-id="5cbd5-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-132">The following is an example of the response.</span></span> 

><span data-ttu-id="5cbd5-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cbd5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5cbd5-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5cbd5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5cbd5-136">C#</span><span class="sxs-lookup"><span data-stu-id="5cbd5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cbd5-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="5cbd5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsignindetailedsummary-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsignindetailedsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
