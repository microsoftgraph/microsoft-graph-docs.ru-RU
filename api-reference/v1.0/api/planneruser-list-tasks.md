---
title: Перечисление задач
description: Получение списка объектов **plannertask**, назначенных объекту User.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 18bd1fae45c75f15e5ed5661253dca4a388e02c9
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473313"
---
# <a name="list-tasks"></a><span data-ttu-id="f6563-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="f6563-103">List tasks</span></span>

<span data-ttu-id="f6563-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6563-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6563-105">Получение списка объектов **plannertask**, назначенных объекту User.</span><span class="sxs-lookup"><span data-stu-id="f6563-105">Retrieve a list of **plannertask** objects assigned to a User.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6563-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6563-106">Permissions</span></span>
<span data-ttu-id="f6563-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6563-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6563-109">Permission type</span></span>      | <span data-ttu-id="f6563-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6563-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6563-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6563-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6563-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6563-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6563-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6563-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6563-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6563-114">Not supported.</span></span>    |
|<span data-ttu-id="f6563-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6563-115">Application</span></span> | <span data-ttu-id="f6563-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6563-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6563-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6563-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/tasks
GET /users/{id}/planner/tasks
GET /drive/root/createdByUser/planner/tasks
```

## <a name="request-headers"></a><span data-ttu-id="f6563-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6563-118">Request headers</span></span>
| <span data-ttu-id="f6563-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f6563-119">Name</span></span>      |<span data-ttu-id="f6563-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6563-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6563-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6563-121">Authorization</span></span>  | <span data-ttu-id="f6563-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6563-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6563-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6563-124">Request body</span></span>
<span data-ttu-id="f6563-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6563-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6563-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6563-126">Response</span></span>

<span data-ttu-id="f6563-127">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f6563-127">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="f6563-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f6563-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f6563-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f6563-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6563-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6563-132">Request</span></span>
<span data-ttu-id="f6563-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6563-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6563-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6563-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "planneruser_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/planner/tasks
```
# <a name="c"></a>[<span data-ttu-id="f6563-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6563-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/planneruser-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6563-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6563-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/planneruser-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6563-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6563-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/planneruser-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6563-138">Java</span><span class="sxs-lookup"><span data-stu-id="f6563-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/planneruser-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f6563-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6563-139">Response</span></span>
<span data-ttu-id="f6563-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6563-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

