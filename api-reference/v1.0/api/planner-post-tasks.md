---
title: Создание объекта plannerTask
description: Используйте этот API, чтобы создать объект **plannerTask**.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9d38c5e4c245e33343a3ea6488699d4da3f43ce7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054499"
---
# <a name="create-plannertask"></a><span data-ttu-id="0d7d9-103">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="0d7d9-103">Create plannerTask</span></span>

<span data-ttu-id="0d7d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d7d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d7d9-105">Используйте этот API, чтобы создать объект **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-105">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d7d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d7d9-106">Permissions</span></span>
<span data-ttu-id="0d7d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d7d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d7d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d7d9-109">Permission type</span></span>      | <span data-ttu-id="0d7d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d7d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d7d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d7d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d7d9-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d7d9-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d7d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d7d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d7d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-114">Not supported.</span></span>    |
|<span data-ttu-id="0d7d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d7d9-115">Application</span></span> | <span data-ttu-id="0d7d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d7d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d7d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks
```
## <a name="request-headers"></a><span data-ttu-id="0d7d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d7d9-118">Request headers</span></span>
| <span data-ttu-id="0d7d9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0d7d9-119">Name</span></span>       | <span data-ttu-id="0d7d9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0d7d9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d7d9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d7d9-121">Authorization</span></span>  | <span data-ttu-id="0d7d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d7d9-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d7d9-124">Request body</span></span>
<span data-ttu-id="0d7d9-p103">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON. В качестве свойства **задачи Планировщика** planId необходимо указать идентификатор существующего объекта [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="0d7d9-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="0d7d9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d7d9-127">Response</span></span>

<span data-ttu-id="0d7d9-128">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-128">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="0d7d9-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0d7d9-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0d7d9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0d7d9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d7d9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d7d9-133">Request</span></span>
<span data-ttu-id="0d7d9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d7d9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7d9-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="0d7d9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d7d9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0d7d9-137">C#</span><span class="sxs-lookup"><span data-stu-id="0d7d9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannertask-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0d7d9-138">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-138">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0d7d9-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d7d9-139">Response</span></span>
<span data-ttu-id="0d7d9-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-140">Here is an example of the response.</span></span> <span data-ttu-id="0d7d9-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0d7d9-141">Note: The response object shown here might be shortened for readability.</span></span>
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

