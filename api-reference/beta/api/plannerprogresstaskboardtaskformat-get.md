---
title: Получение объекта plannerProgressTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1a8e6bbf1c56ffb966151931925572747fb5b47a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979029"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="516e9-103">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="516e9-103">Get plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516e9-104">Получение свойств и связей объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="516e9-104">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="516e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="516e9-105">Permissions</span></span>
<span data-ttu-id="516e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="516e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="516e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="516e9-108">Permission type</span></span>      | <span data-ttu-id="516e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="516e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="516e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="516e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="516e9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="516e9-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="516e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="516e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516e9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="516e9-113">Not supported.</span></span>    |
|<span data-ttu-id="516e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="516e9-114">Application</span></span> | <span data-ttu-id="516e9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="516e9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="516e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="516e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="516e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="516e9-117">Request headers</span></span>
| <span data-ttu-id="516e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="516e9-118">Name</span></span>      |<span data-ttu-id="516e9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="516e9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="516e9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="516e9-120">Authorization</span></span>  | <span data-ttu-id="516e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="516e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="516e9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="516e9-123">Request body</span></span>
<span data-ttu-id="516e9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="516e9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="516e9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="516e9-125">Response</span></span>

<span data-ttu-id="516e9-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="516e9-126">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="516e9-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="516e9-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="516e9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="516e9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="516e9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="516e9-131">Request</span></span>
<span data-ttu-id="516e9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="516e9-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="516e9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="516e9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="516e9-134">C#</span><span class="sxs-lookup"><span data-stu-id="516e9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="516e9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="516e9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="516e9-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="516e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="516e9-137">Java</span><span class="sxs-lookup"><span data-stu-id="516e9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="516e9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="516e9-138">Response</span></span>
<span data-ttu-id="516e9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="516e9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
