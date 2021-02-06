---
title: Получение applicationSignInDetailedSummary
description: Получение свойств и связей объекта applicationSignInDetailSummary.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 17f4a087d548ae06b69430c3ca442ead5ac38625
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128990"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="c9ee6-103">Получение applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="c9ee6-103">Get applicationSignInDetailedSummary</span></span>

<span data-ttu-id="c9ee6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9ee6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ee6-105">Получение свойств и связей объекта [applicationSignInDetailSummary.](../resources/applicationsignindetailedsummary.md)</span><span class="sxs-lookup"><span data-stu-id="c9ee6-105">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9ee6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ee6-106">Permissions</span></span>
<span data-ttu-id="c9ee6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9ee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="c9ee6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ee6-109">Permission type</span></span>                        | <span data-ttu-id="c9ee6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9ee6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9ee6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9ee6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9ee6-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9ee6-112">Report.Read.All</span></span> |
|<span data-ttu-id="c9ee6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9ee6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ee6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-114">Not supported.</span></span> |
|<span data-ttu-id="c9ee6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9ee6-115">Application</span></span>                            | <span data-ttu-id="c9ee6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9ee6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9ee6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9ee6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9ee6-118">Optional query parameters</span></span>

<span data-ttu-id="c9ee6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9ee6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9ee6-120">Request headers</span></span>

| <span data-ttu-id="c9ee6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c9ee6-121">Name</span></span>      |<span data-ttu-id="c9ee6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c9ee6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9ee6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9ee6-123">Authorization</span></span> | <span data-ttu-id="c9ee6-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c9ee6-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9ee6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9ee6-125">Request body</span></span>
<span data-ttu-id="c9ee6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9ee6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ee6-127">Response</span></span>
<span data-ttu-id="c9ee6-128">В случае успеха этот метод возвращает код отклика и объект `200 OK` [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-128">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9ee6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c9ee6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9ee6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9ee6-130">Request</span></span>
<span data-ttu-id="c9ee6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9ee6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9ee6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="c"></a>[<span data-ttu-id="c9ee6-133">C#</span><span class="sxs-lookup"><span data-stu-id="c9ee6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9ee6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9ee6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9ee6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9ee6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9ee6-136">Java</span><span class="sxs-lookup"><span data-stu-id="c9ee6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9ee6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ee6-137">Response</span></span>
<span data-ttu-id="c9ee6-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c9ee6-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9ee6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


