---
title: Получение объекта plannerProgressTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 644066685ecb8fcc17dfe3bc2df59c05271352cd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050012"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="9133e-103">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9133e-103">Get plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="9133e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9133e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9133e-105">Получение свойств и связей объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="9133e-105">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9133e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9133e-106">Permissions</span></span>
<span data-ttu-id="9133e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9133e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9133e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9133e-109">Permission type</span></span>      | <span data-ttu-id="9133e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9133e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9133e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9133e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9133e-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9133e-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9133e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9133e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9133e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9133e-114">Not supported.</span></span>    |
|<span data-ttu-id="9133e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9133e-115">Application</span></span> | <span data-ttu-id="9133e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9133e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9133e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9133e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="9133e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9133e-118">Request headers</span></span>
| <span data-ttu-id="9133e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9133e-119">Name</span></span>      |<span data-ttu-id="9133e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9133e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9133e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9133e-121">Authorization</span></span>  | <span data-ttu-id="9133e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9133e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9133e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9133e-124">Request body</span></span>
<span data-ttu-id="9133e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9133e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9133e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9133e-126">Response</span></span>

<span data-ttu-id="9133e-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9133e-127">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="9133e-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9133e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9133e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9133e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9133e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9133e-132">Request</span></span>
<span data-ttu-id="9133e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9133e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9133e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9133e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="9133e-135">C#</span><span class="sxs-lookup"><span data-stu-id="9133e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9133e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9133e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9133e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9133e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9133e-138">Java</span><span class="sxs-lookup"><span data-stu-id="9133e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9133e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9133e-139">Response</span></span>
<span data-ttu-id="9133e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9133e-140">Here is an example of the response.</span></span> <span data-ttu-id="9133e-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9133e-141">Note: The response object shown here might be shortened for readability.</span></span>
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


