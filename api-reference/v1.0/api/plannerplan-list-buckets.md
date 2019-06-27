---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**, содержащихся в объекте plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d45affbb0ee9e1382312cb4977a1472e030ed721
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276547"
---
# <a name="list-buckets"></a><span data-ttu-id="dcef7-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="dcef7-103">List buckets</span></span>

<span data-ttu-id="dcef7-104">Получение списка объектов **plannerbucket**, содержащихся в объекте [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="dcef7-104">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dcef7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcef7-105">Permissions</span></span>
<span data-ttu-id="dcef7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcef7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcef7-108">Permission type</span></span>      | <span data-ttu-id="dcef7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcef7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcef7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcef7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcef7-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcef7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dcef7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcef7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcef7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcef7-113">Not supported.</span></span>    |
|<span data-ttu-id="dcef7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcef7-114">Application</span></span> | <span data-ttu-id="dcef7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcef7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcef7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcef7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="dcef7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcef7-117">Request headers</span></span>
| <span data-ttu-id="dcef7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dcef7-118">Name</span></span>      |<span data-ttu-id="dcef7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dcef7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcef7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcef7-120">Authorization</span></span>  | <span data-ttu-id="dcef7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcef7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcef7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dcef7-123">Request body</span></span>
<span data-ttu-id="dcef7-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dcef7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcef7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="dcef7-125">Response</span></span>

<span data-ttu-id="dcef7-126">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dcef7-126">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="dcef7-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="dcef7-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="dcef7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dcef7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcef7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcef7-131">Request</span></span>
<span data-ttu-id="dcef7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcef7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="dcef7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcef7-133">Response</span></span>
<span data-ttu-id="dcef7-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcef7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dcef7-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dcef7-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dcef7-138">C#</span><span class="sxs-lookup"><span data-stu-id="dcef7-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_buckets-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcef7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcef7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_buckets-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dcef7-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dcef7-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_buckets-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-list-buckets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
