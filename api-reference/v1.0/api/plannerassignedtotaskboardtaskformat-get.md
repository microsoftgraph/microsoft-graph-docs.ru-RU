---
title: Получение объекта plannerAssignedToTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: abad4d469289c63d979b7a0a5a31b41c4afc8756
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035185"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="f9ebf-103">Получение объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f9ebf-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="f9ebf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ebf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9ebf-105">Получение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-105">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9ebf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ebf-106">Permissions</span></span>
<span data-ttu-id="f9ebf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ebf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ebf-109">Permission type</span></span>      | <span data-ttu-id="f9ebf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9ebf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ebf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9ebf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ebf-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ebf-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9ebf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9ebf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ebf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-114">Not supported.</span></span>    |
|<span data-ttu-id="f9ebf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9ebf-115">Application</span></span> | <span data-ttu-id="f9ebf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ebf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9ebf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="f9ebf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9ebf-118">Request headers</span></span>
| <span data-ttu-id="f9ebf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f9ebf-119">Name</span></span>      |<span data-ttu-id="f9ebf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ebf-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9ebf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9ebf-121">Authorization</span></span>  | <span data-ttu-id="f9ebf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9ebf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9ebf-124">Request body</span></span>
<span data-ttu-id="f9ebf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ebf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ebf-126">Response</span></span>

<span data-ttu-id="f9ebf-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-127">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="f9ebf-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f9ebf-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f9ebf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f9ebf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9ebf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9ebf-132">Request</span></span>
<span data-ttu-id="f9ebf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9ebf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ebf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="f9ebf-135">C#</span><span class="sxs-lookup"><span data-stu-id="f9ebf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9ebf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9ebf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9ebf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9ebf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9ebf-138">Java</span><span class="sxs-lookup"><span data-stu-id="f9ebf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerassignedtotaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9ebf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ebf-139">Response</span></span>
<span data-ttu-id="f9ebf-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-140">Here is an example of the response.</span></span> <span data-ttu-id="f9ebf-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f9ebf-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

