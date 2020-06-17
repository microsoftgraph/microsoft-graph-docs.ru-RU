---
title: Создание объекта plannerTask
description: Используйте этот API, чтобы создать объект **plannerTask**.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a7800ee4331b3a81a16accd2d01f132a53bc511d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681693"
---
# <a name="create-plannertask"></a><span data-ttu-id="cf562-103">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="cf562-103">Create plannerTask</span></span>

<span data-ttu-id="cf562-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf562-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf562-105">Используйте этот API, чтобы создать объект **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="cf562-105">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf562-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf562-106">Permissions</span></span>
<span data-ttu-id="cf562-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cf562-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cf562-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf562-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf562-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf562-109">Permission type</span></span>      | <span data-ttu-id="cf562-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf562-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf562-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf562-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf562-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf562-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf562-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf562-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf562-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf562-114">Not supported.</span></span>    |
|<span data-ttu-id="cf562-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf562-115">Application</span></span> | <span data-ttu-id="cf562-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf562-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf562-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf562-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks
```
## <a name="request-headers"></a><span data-ttu-id="cf562-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf562-118">Request headers</span></span>
| <span data-ttu-id="cf562-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cf562-119">Name</span></span>       | <span data-ttu-id="cf562-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cf562-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf562-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf562-121">Authorization</span></span>  | <span data-ttu-id="cf562-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="cf562-122">Bearer {token}.</span></span> <span data-ttu-id="cf562-123">Required.</span><span class="sxs-lookup"><span data-stu-id="cf562-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf562-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf562-124">Request body</span></span>
<span data-ttu-id="cf562-125">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span><span class="sxs-lookup"><span data-stu-id="cf562-125">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
<span data-ttu-id="cf562-126">The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span><span class="sxs-lookup"><span data-stu-id="cf562-126">The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="cf562-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf562-127">Response</span></span>

<span data-ttu-id="cf562-128">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf562-128">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="cf562-129">This method can return any of the [HTTP status codes](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="cf562-129">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="cf562-130">The most common errors that apps should handle for this method are the 400, 403 and 404 responses.</span><span class="sxs-lookup"><span data-stu-id="cf562-130">The most common errors that apps should handle for this method are the 400, 403 and 404 responses.</span></span> <span data-ttu-id="cf562-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="cf562-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="cf562-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cf562-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf562-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf562-133">Request</span></span>
<span data-ttu-id="cf562-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf562-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf562-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf562-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="cf562-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf562-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf562-137">C#</span><span class="sxs-lookup"><span data-stu-id="cf562-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannertask-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cf562-138">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf562-138">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cf562-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf562-139">Response</span></span>
<span data-ttu-id="cf562-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="cf562-140">Here is an example of the response.</span></span> <span data-ttu-id="cf562-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="cf562-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cf562-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cf562-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
