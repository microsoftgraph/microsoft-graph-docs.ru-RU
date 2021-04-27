---
title: Получение объекта plannerTask
description: Получение свойств и связей объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d7b6500ae85214f6eb6608f8ebba14632346fa76
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049991"
---
# <a name="get-plannertask"></a><span data-ttu-id="1c30f-103">Получение объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="1c30f-103">Get plannerTask</span></span>

<span data-ttu-id="1c30f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c30f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c30f-105">Получение свойств и связей объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="1c30f-105">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c30f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c30f-106">Permissions</span></span>
<span data-ttu-id="1c30f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c30f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c30f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c30f-109">Permission type</span></span>      | <span data-ttu-id="1c30f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c30f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c30f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c30f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c30f-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c30f-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c30f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c30f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c30f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c30f-114">Not supported.</span></span>    |
|<span data-ttu-id="1c30f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c30f-115">Application</span></span> | <span data-ttu-id="1c30f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c30f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c30f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c30f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c30f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c30f-118">Request headers</span></span>
| <span data-ttu-id="1c30f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1c30f-119">Name</span></span>      |<span data-ttu-id="1c30f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c30f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c30f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c30f-121">Authorization</span></span>  | <span data-ttu-id="1c30f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c30f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c30f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c30f-124">Request body</span></span>
<span data-ttu-id="1c30f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c30f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c30f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c30f-126">Response</span></span>

<span data-ttu-id="1c30f-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1c30f-127">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="1c30f-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="1c30f-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="1c30f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1c30f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c30f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c30f-132">Request</span></span>
<span data-ttu-id="1c30f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c30f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c30f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c30f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
```
# <a name="c"></a>[<span data-ttu-id="1c30f-135">C#</span><span class="sxs-lookup"><span data-stu-id="1c30f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c30f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c30f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c30f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c30f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c30f-138">Java</span><span class="sxs-lookup"><span data-stu-id="1c30f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c30f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c30f-139">Response</span></span>
<span data-ttu-id="1c30f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c30f-140">Here is an example of the response.</span></span> <span data-ttu-id="1c30f-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c30f-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
  "title": "title-value",
  "orderHint": "9223370609546166567W",
  "assigneePriority": "90057581\"",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


