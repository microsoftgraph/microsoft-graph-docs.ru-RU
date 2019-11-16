---
title: Перечисление задач
description: Получение списка объектов **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 14f4910e56e05f049d9ccf397427a5f4a714164a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37633826"
---
# <a name="list-tasks"></a><span data-ttu-id="737e8-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="737e8-103">List tasks</span></span>

<span data-ttu-id="737e8-104">Получение списка объектов **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="737e8-104">Retrieve a list of **plannertask** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="737e8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="737e8-105">Permissions</span></span>
<span data-ttu-id="737e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="737e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="737e8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="737e8-108">Permission type</span></span>      | <span data-ttu-id="737e8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="737e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="737e8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="737e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="737e8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="737e8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="737e8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="737e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="737e8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737e8-113">Not supported.</span></span>    |
|<span data-ttu-id="737e8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="737e8-114">Application</span></span> | <span data-ttu-id="737e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="737e8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="737e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="737e8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="737e8-117">Optional query parameters</span></span>
<span data-ttu-id="737e8-118">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по идентификатору плана.</span><span class="sxs-lookup"><span data-stu-id="737e8-118">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="737e8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="737e8-119">Request headers</span></span>
| <span data-ttu-id="737e8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="737e8-120">Name</span></span>      |<span data-ttu-id="737e8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="737e8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="737e8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="737e8-122">Authorization</span></span>  | <span data-ttu-id="737e8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="737e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="737e8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="737e8-125">Request body</span></span>
<span data-ttu-id="737e8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="737e8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="737e8-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="737e8-127">Response</span></span>

<span data-ttu-id="737e8-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="737e8-128">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="737e8-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="737e8-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="737e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="737e8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="737e8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="737e8-133">Request</span></span>
<span data-ttu-id="737e8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="737e8-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="737e8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="737e8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planner_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="737e8-136">C#</span><span class="sxs-lookup"><span data-stu-id="737e8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planner-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="737e8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="737e8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planner-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="737e8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="737e8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planner-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="737e8-139">Java</span><span class="sxs-lookup"><span data-stu-id="737e8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/planner-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="737e8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="737e8-140">Response</span></span>
<span data-ttu-id="737e8-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="737e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
