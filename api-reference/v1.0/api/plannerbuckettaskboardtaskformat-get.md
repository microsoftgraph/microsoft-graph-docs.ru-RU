---
title: Получение объекта plannerBucketTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4ffba6b8fc8f68015f43e2de32bb2053dbf72b1b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275476"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="791a8-103">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="791a8-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="791a8-104">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="791a8-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="791a8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="791a8-105">Permissions</span></span>
<span data-ttu-id="791a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791a8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791a8-108">Permission type</span></span>      | <span data-ttu-id="791a8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="791a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="791a8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="791a8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791a8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="791a8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791a8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791a8-113">Not supported.</span></span>    |
|<span data-ttu-id="791a8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791a8-114">Application</span></span> | <span data-ttu-id="791a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791a8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="791a8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="791a8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="791a8-117">Request headers</span></span>
| <span data-ttu-id="791a8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="791a8-118">Name</span></span>      |<span data-ttu-id="791a8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="791a8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="791a8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="791a8-120">Authorization</span></span>  | <span data-ttu-id="791a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="791a8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="791a8-123">Request body</span></span>
<span data-ttu-id="791a8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="791a8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="791a8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="791a8-125">Response</span></span>

<span data-ttu-id="791a8-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="791a8-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="791a8-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="791a8-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="791a8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="791a8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="791a8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="791a8-131">Request</span></span>
<span data-ttu-id="791a8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="791a8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="791a8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="791a8-133">Response</span></span>
<span data-ttu-id="791a8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="791a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="791a8-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="791a8-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="791a8-138">C#</span><span class="sxs-lookup"><span data-stu-id="791a8-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="791a8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="791a8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="791a8-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="791a8-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_plannerbuckettaskboardtaskformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerbuckettaskboardtaskformat-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
