---
title: Получение объекта plannerBucketTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e1490fe8de9ddff150843a0e206a850192a969af
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725761"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="49247-103">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="49247-103">Get plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49247-104">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="49247-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49247-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49247-105">Permissions</span></span>
<span data-ttu-id="49247-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49247-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49247-108">Permission type</span></span>      | <span data-ttu-id="49247-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49247-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49247-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49247-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49247-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49247-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49247-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49247-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49247-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49247-113">Not supported.</span></span>    |
|<span data-ttu-id="49247-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49247-114">Application</span></span> | <span data-ttu-id="49247-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49247-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49247-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49247-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="49247-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49247-117">Request headers</span></span>
| <span data-ttu-id="49247-118">Имя</span><span class="sxs-lookup"><span data-stu-id="49247-118">Name</span></span>      |<span data-ttu-id="49247-119">Описание</span><span class="sxs-lookup"><span data-stu-id="49247-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49247-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49247-120">Authorization</span></span>  | <span data-ttu-id="49247-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49247-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49247-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49247-123">Request body</span></span>
<span data-ttu-id="49247-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49247-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49247-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="49247-125">Response</span></span>

<span data-ttu-id="49247-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49247-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="49247-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="49247-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="49247-130">Пример</span><span class="sxs-lookup"><span data-stu-id="49247-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49247-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="49247-131">Request</span></span>
<span data-ttu-id="49247-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49247-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49247-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="49247-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49247-134">C#</span><span class="sxs-lookup"><span data-stu-id="49247-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49247-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49247-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49247-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="49247-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49247-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="49247-137">Response</span></span>
<span data-ttu-id="49247-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49247-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
