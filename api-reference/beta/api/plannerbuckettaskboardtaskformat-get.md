---
title: Получение объекта plannerBucketTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 86f4b7f908159957258ad9485fdd6f3e964404a2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978291"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="72ceb-103">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="72ceb-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="72ceb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72ceb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ceb-105">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="72ceb-105">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72ceb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72ceb-106">Permissions</span></span>
<span data-ttu-id="72ceb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72ceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72ceb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72ceb-109">Permission type</span></span>      | <span data-ttu-id="72ceb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72ceb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72ceb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72ceb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72ceb-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72ceb-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="72ceb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72ceb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72ceb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ceb-114">Not supported.</span></span>    |
|<span data-ttu-id="72ceb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72ceb-115">Application</span></span> | <span data-ttu-id="72ceb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72ceb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72ceb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72ceb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="72ceb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72ceb-118">Request headers</span></span>
| <span data-ttu-id="72ceb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72ceb-119">Name</span></span>      |<span data-ttu-id="72ceb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72ceb-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72ceb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72ceb-121">Authorization</span></span>  | <span data-ttu-id="72ceb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72ceb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72ceb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72ceb-124">Request body</span></span>
<span data-ttu-id="72ceb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72ceb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72ceb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ceb-126">Response</span></span>

<span data-ttu-id="72ceb-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72ceb-127">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="72ceb-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="72ceb-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="72ceb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="72ceb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72ceb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="72ceb-132">Request</span></span>
<span data-ttu-id="72ceb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72ceb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72ceb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="72ceb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="c"></a>[<span data-ttu-id="72ceb-135">C#</span><span class="sxs-lookup"><span data-stu-id="72ceb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72ceb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72ceb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72ceb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72ceb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72ceb-138">Java</span><span class="sxs-lookup"><span data-stu-id="72ceb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72ceb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="72ceb-139">Response</span></span>
<span data-ttu-id="72ceb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72ceb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


