---
title: Перечисление задач
description: Получение списка объектов **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 15b27dce703c8e8e23742252584181d35911ce69
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055367"
---
# <a name="list-tasks"></a><span data-ttu-id="832ce-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="832ce-103">List tasks</span></span>

<span data-ttu-id="832ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="832ce-105">Получение списка объектов **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="832ce-105">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="832ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="832ce-106">Permissions</span></span>
<span data-ttu-id="832ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="832ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="832ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="832ce-109">Permission type</span></span>      | <span data-ttu-id="832ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="832ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="832ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="832ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="832ce-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="832ce-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="832ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="832ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="832ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="832ce-114">Not supported.</span></span>    |
|<span data-ttu-id="832ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="832ce-115">Application</span></span> | <span data-ttu-id="832ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="832ce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="832ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="832ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="832ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="832ce-118">Optional query parameters</span></span>
<span data-ttu-id="832ce-119">Этот метод требует указания [фильтра](/graph/query-parameters) по идентификатору плана.</span><span class="sxs-lookup"><span data-stu-id="832ce-119">This method requires planId [filter](/graph/query-parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="832ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="832ce-120">Request headers</span></span>
| <span data-ttu-id="832ce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="832ce-121">Name</span></span>      |<span data-ttu-id="832ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="832ce-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="832ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="832ce-123">Authorization</span></span>  | <span data-ttu-id="832ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="832ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="832ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="832ce-126">Request body</span></span>
<span data-ttu-id="832ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="832ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="832ce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="832ce-128">Response</span></span>

<span data-ttu-id="832ce-129">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="832ce-129">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="832ce-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="832ce-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="832ce-133">Пример</span><span class="sxs-lookup"><span data-stu-id="832ce-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="832ce-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="832ce-134">Request</span></span>
<span data-ttu-id="832ce-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="832ce-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="832ce-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="832ce-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planner_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks
```
# <a name="c"></a>[<span data-ttu-id="832ce-137">C#</span><span class="sxs-lookup"><span data-stu-id="832ce-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planner-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="832ce-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="832ce-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planner-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="832ce-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="832ce-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planner-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="832ce-140">Java</span><span class="sxs-lookup"><span data-stu-id="832ce-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/planner-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="832ce-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="832ce-141">Response</span></span>
<span data-ttu-id="832ce-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="832ce-142">Here is an example of the response.</span></span> <span data-ttu-id="832ce-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="832ce-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
