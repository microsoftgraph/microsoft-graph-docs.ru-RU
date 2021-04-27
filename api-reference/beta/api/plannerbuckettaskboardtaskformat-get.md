---
title: Получение объекта plannerBucketTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a9b3faa8f2662324f31ab4843781ba3dfc54c250
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052049"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="bb763-103">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="bb763-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="bb763-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb763-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb763-105">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="bb763-105">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb763-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb763-106">Permissions</span></span>
<span data-ttu-id="bb763-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb763-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb763-109">Permission type</span></span>      | <span data-ttu-id="bb763-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb763-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb763-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb763-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb763-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb763-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb763-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb763-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb763-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb763-114">Not supported.</span></span>    |
|<span data-ttu-id="bb763-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb763-115">Application</span></span> | <span data-ttu-id="bb763-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb763-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb763-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb763-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="bb763-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb763-118">Request headers</span></span>
| <span data-ttu-id="bb763-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bb763-119">Name</span></span>      |<span data-ttu-id="bb763-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bb763-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb763-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb763-121">Authorization</span></span>  | <span data-ttu-id="bb763-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb763-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb763-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb763-124">Request body</span></span>
<span data-ttu-id="bb763-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb763-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb763-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb763-126">Response</span></span>

<span data-ttu-id="bb763-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb763-127">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="bb763-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bb763-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bb763-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb763-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb763-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb763-132">Request</span></span>
<span data-ttu-id="bb763-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb763-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb763-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb763-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="bb763-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb763-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb763-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb763-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb763-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb763-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb763-138">Java</span><span class="sxs-lookup"><span data-stu-id="bb763-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb763-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb763-139">Response</span></span>
<span data-ttu-id="bb763-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb763-140">Here is an example of the response.</span></span> <span data-ttu-id="bb763-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb763-141">Note: The response object shown here might be shortened for readability.</span></span>
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


