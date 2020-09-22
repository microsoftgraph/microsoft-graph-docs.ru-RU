---
title: Перечисление задач
description: Получение списка объектов **plannerTask** , связанных с объектом plannerPlan.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c50b84fce3773d9b9e50fd1e85998f2af74b6fc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020690"
---
# <a name="list-tasks"></a><span data-ttu-id="c3a4e-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="c3a4e-103">List tasks</span></span>

<span data-ttu-id="c3a4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3a4e-105">Получение списка объектов [plannerTask](../resources/plannertask.md) , связанных с объектом [plannerPlan](../resources/plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="c3a4e-105">Retrieve a list of [plannerTask](../resources/plannertask.md) objects associated with a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3a4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3a4e-106">Permissions</span></span>
<span data-ttu-id="c3a4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3a4e-109">Permission type</span></span>      | <span data-ttu-id="c3a4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3a4e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3a4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3a4e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3a4e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a4e-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3a4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3a4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3a4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-114">Not supported.</span></span>    |
|<span data-ttu-id="c3a4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3a4e-115">Application</span></span> | <span data-ttu-id="c3a4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3a4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3a4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="c3a4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3a4e-118">Request headers</span></span>
| <span data-ttu-id="c3a4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c3a4e-119">Name</span></span>      |<span data-ttu-id="c3a4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a4e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3a4e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3a4e-121">Authorization</span></span>  | <span data-ttu-id="c3a4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3a4e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3a4e-124">Request body</span></span>
<span data-ttu-id="c3a4e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3a4e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a4e-126">Response</span></span>

<span data-ttu-id="c3a4e-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-127">If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="c3a4e-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c3a4e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c3a4e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a4e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3a4e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a4e-132">Request</span></span>
<span data-ttu-id="c3a4e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3a4e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3a4e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "plannerplan_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/tasks
```
# <a name="c"></a>[<span data-ttu-id="c3a4e-135">C#</span><span class="sxs-lookup"><span data-stu-id="c3a4e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/plannerplan-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3a4e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3a4e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/plannerplan-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3a4e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3a4e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/plannerplan-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3a4e-138">Java</span><span class="sxs-lookup"><span data-stu-id="c3a4e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/plannerplan-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3a4e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a4e-139">Response</span></span>
<span data-ttu-id="c3a4e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-140">Here is an example of the response.</span></span> 

><span data-ttu-id="c3a4e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3a4e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

