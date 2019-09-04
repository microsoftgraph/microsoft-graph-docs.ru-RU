---
title: Получение Аппликатионсигниндетаиледсуммари
description: Получение свойств и связей объекта Аппликатионсигниндетаилсуммари.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb350aaf532ec66a3788fe6b2168249c2ae5e028
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719017"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="423c7-103">Получение Аппликатионсигниндетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="423c7-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="423c7-104">Получение свойств и связей объекта [аппликатионсигниндетаилсуммари](../resources/applicationsignindetailedsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="423c7-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="423c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="423c7-105">Permissions</span></span>
<span data-ttu-id="423c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="423c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="423c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="423c7-108">Permission type</span></span>                        | <span data-ttu-id="423c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="423c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="423c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="423c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="423c7-111">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="423c7-111">Report.Read.All</span></span> |
|<span data-ttu-id="423c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="423c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="423c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423c7-113">Not supported.</span></span> |
|<span data-ttu-id="423c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="423c7-114">Application</span></span>                            | <span data-ttu-id="423c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="423c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="423c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="423c7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="423c7-117">Optional query parameters</span></span>

<span data-ttu-id="423c7-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="423c7-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="423c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="423c7-119">Request headers</span></span>

| <span data-ttu-id="423c7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="423c7-120">Name</span></span>      |<span data-ttu-id="423c7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="423c7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="423c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="423c7-122">Authorization</span></span> | <span data-ttu-id="423c7-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="423c7-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="423c7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="423c7-124">Request body</span></span>
<span data-ttu-id="423c7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="423c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="423c7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="423c7-126">Response</span></span>
<span data-ttu-id="423c7-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аппликатионсигниндетаиледсуммари](../resources/applicationsignindetailedsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="423c7-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="423c7-128">Пример</span><span class="sxs-lookup"><span data-stu-id="423c7-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="423c7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="423c7-129">Request</span></span>
<span data-ttu-id="423c7-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="423c7-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="423c7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="423c7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="423c7-132">C#</span><span class="sxs-lookup"><span data-stu-id="423c7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="423c7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="423c7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="423c7-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="423c7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="423c7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="423c7-135">Response</span></span>
<span data-ttu-id="423c7-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="423c7-136">The following is an example of the response.</span></span> 

><span data-ttu-id="423c7-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="423c7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
