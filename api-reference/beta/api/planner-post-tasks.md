---
title: Создание объекта plannerTask
description: Используйте этот API, чтобы создать объект **plannerTask**.
localization_priority: Normal
ms.openlocfilehash: a883e6d3760f40f7e633df7a99bb76a17e91b13b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831838"
---
# <a name="create-plannertask"></a><span data-ttu-id="c17fc-103">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="c17fc-103">Create plannerTask</span></span>

> <span data-ttu-id="c17fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c17fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c17fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c17fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c17fc-106">Используйте этот API, чтобы создать объект **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="c17fc-106">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="c17fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c17fc-107">Permissions</span></span>
<span data-ttu-id="c17fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c17fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c17fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c17fc-110">Permission type</span></span>      | <span data-ttu-id="c17fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c17fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c17fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c17fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c17fc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c17fc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c17fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c17fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c17fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c17fc-115">Not supported.</span></span>    |
|<span data-ttu-id="c17fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c17fc-116">Application</span></span> | <span data-ttu-id="c17fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c17fc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c17fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c17fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks

```
## <a name="request-headers"></a><span data-ttu-id="c17fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c17fc-119">Request headers</span></span>
| <span data-ttu-id="c17fc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c17fc-120">Name</span></span>       | <span data-ttu-id="c17fc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c17fc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c17fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c17fc-122">Authorization</span></span>  | <span data-ttu-id="c17fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c17fc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c17fc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c17fc-125">Request body</span></span>
<span data-ttu-id="c17fc-p104">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON. В качестве свойства **задачи Планировщика** planId необходимо указать идентификатор существующего объекта [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="c17fc-p104">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object. The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="c17fc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c17fc-128">Response</span></span>

<span data-ttu-id="c17fc-129">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c17fc-129">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="c17fc-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c17fc-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c17fc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c17fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c17fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c17fc-134">Request</span></span>
<span data-ttu-id="c17fc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c17fc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/beta/planner/tasks
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
<span data-ttu-id="c17fc-136">Включите в текст запроса описание объекта [plannerTask](../resources/plannertask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c17fc-136">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c17fc-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c17fc-137">Response</span></span>
<span data-ttu-id="c17fc-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c17fc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
