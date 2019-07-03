---
title: Создание объекта plannerTask
description: Используйте этот API, чтобы создать объект **plannerTask**.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9c62ce0ff48154fe848e01f6405109ba1266a76d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455457"
---
# <a name="create-plannertask"></a><span data-ttu-id="48ded-103">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="48ded-103">Create plannerTask</span></span>

<span data-ttu-id="48ded-104">Используйте этот API, чтобы создать объект **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="48ded-104">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="48ded-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48ded-105">Permissions</span></span>
<span data-ttu-id="48ded-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48ded-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48ded-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48ded-108">Permission type</span></span>      | <span data-ttu-id="48ded-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48ded-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48ded-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48ded-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48ded-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48ded-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48ded-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48ded-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48ded-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48ded-113">Not supported.</span></span>    |
|<span data-ttu-id="48ded-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48ded-114">Application</span></span> | <span data-ttu-id="48ded-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48ded-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48ded-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48ded-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="48ded-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48ded-117">Request headers</span></span>
| <span data-ttu-id="48ded-118">Имя</span><span class="sxs-lookup"><span data-stu-id="48ded-118">Name</span></span>       | <span data-ttu-id="48ded-119">Описание</span><span class="sxs-lookup"><span data-stu-id="48ded-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48ded-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48ded-120">Authorization</span></span>  | <span data-ttu-id="48ded-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48ded-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48ded-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48ded-123">Request body</span></span>
<span data-ttu-id="48ded-p103">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON. В качестве свойства **задачи Планировщика** planId необходимо указать идентификатор существующего объекта [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="48ded-p103">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="48ded-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="48ded-126">Response</span></span>

<span data-ttu-id="48ded-127">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="48ded-127">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="48ded-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="48ded-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="48ded-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48ded-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48ded-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48ded-132">Request</span></span>
<span data-ttu-id="48ded-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48ded-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48ded-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="48ded-134">--Http</span></span>](#tab/http)
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
  },
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48ded-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48ded-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="48ded-136">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48ded-136">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48ded-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="48ded-137">Response</span></span>
<span data-ttu-id="48ded-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48ded-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
