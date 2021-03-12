---
title: Обновление объекта plannertask
description: Обновление свойств объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 410913ba71a7b3404169fbfa2e6f06dcaa47038f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722037"
---
# <a name="update-plannertask"></a><span data-ttu-id="8174f-103">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="8174f-103">Update plannertask</span></span>

<span data-ttu-id="8174f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8174f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8174f-105">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="8174f-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8174f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8174f-106">Permissions</span></span>
<span data-ttu-id="8174f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8174f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8174f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8174f-109">Permission type</span></span>      | <span data-ttu-id="8174f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8174f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8174f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8174f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8174f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8174f-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8174f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8174f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8174f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8174f-114">Not supported.</span></span>    |
|<span data-ttu-id="8174f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8174f-115">Application</span></span> | <span data-ttu-id="8174f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8174f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8174f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8174f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8174f-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8174f-118">Optional request headers</span></span>
| <span data-ttu-id="8174f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8174f-119">Name</span></span>       | <span data-ttu-id="8174f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8174f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8174f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8174f-121">Authorization</span></span>  | <span data-ttu-id="8174f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8174f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8174f-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="8174f-124">If-Match</span></span>  | <span data-ttu-id="8174f-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8174f-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8174f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8174f-127">Request body</span></span>
<span data-ttu-id="8174f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8174f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8174f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8174f-131">Property</span></span>     | <span data-ttu-id="8174f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8174f-132">Type</span></span>   |<span data-ttu-id="8174f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8174f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8174f-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="8174f-134">appliedCategories</span></span>|[<span data-ttu-id="8174f-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="8174f-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="8174f-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="8174f-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="8174f-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="8174f-138">assigneePriority</span></span>|<span data-ttu-id="8174f-139">String</span><span class="sxs-lookup"><span data-stu-id="8174f-139">String</span></span>|<span data-ttu-id="8174f-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="8174f-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="8174f-142">assignments</span><span class="sxs-lookup"><span data-stu-id="8174f-142">assignments</span></span>|[<span data-ttu-id="8174f-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="8174f-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="8174f-144">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="8174f-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="8174f-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="8174f-145">bucketId</span></span>|<span data-ttu-id="8174f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8174f-146">String</span></span>|<span data-ttu-id="8174f-147">Ведерный id, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="8174f-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="8174f-148">Сегмент должен находиться в том же плане, что и задача.</span><span class="sxs-lookup"><span data-stu-id="8174f-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="8174f-149">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8174f-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8174f-150">[Проверка формата](../resources/planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="8174f-150">[Format validation](../resources/planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="8174f-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="8174f-151">conversationThreadId</span></span>|<span data-ttu-id="8174f-152">Строка</span><span class="sxs-lookup"><span data-stu-id="8174f-152">String</span></span>|<span data-ttu-id="8174f-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="8174f-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="8174f-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="8174f-155">dueDateTime</span></span>|<span data-ttu-id="8174f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8174f-156">DateTimeOffset</span></span>|<span data-ttu-id="8174f-157">Дата и время, в которое должна быть поставлена задача.</span><span class="sxs-lookup"><span data-stu-id="8174f-157">Date and time at which the task is due.</span></span> <span data-ttu-id="8174f-158">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8174f-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8174f-159">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8174f-159">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8174f-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="8174f-160">orderHint</span></span>|<span data-ttu-id="8174f-161">String</span><span class="sxs-lookup"><span data-stu-id="8174f-161">String</span></span>|<span data-ttu-id="8174f-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="8174f-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="8174f-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="8174f-164">percentComplete</span></span>|<span data-ttu-id="8174f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8174f-165">Int32</span></span>|<span data-ttu-id="8174f-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="8174f-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="8174f-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8174f-168">startDateTime</span></span>|<span data-ttu-id="8174f-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8174f-169">DateTimeOffset</span></span>|<span data-ttu-id="8174f-170">Дата и время, с которых начинается задача.</span><span class="sxs-lookup"><span data-stu-id="8174f-170">Date and time at which the task starts.</span></span> <span data-ttu-id="8174f-171">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8174f-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8174f-172">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8174f-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8174f-173">title</span><span class="sxs-lookup"><span data-stu-id="8174f-173">title</span></span>|<span data-ttu-id="8174f-174">Строка</span><span class="sxs-lookup"><span data-stu-id="8174f-174">String</span></span>|<span data-ttu-id="8174f-175">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="8174f-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="8174f-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="8174f-176">Response</span></span>

<span data-ttu-id="8174f-177">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8174f-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="8174f-p113">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8174f-p113">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8174f-181">Пример</span><span class="sxs-lookup"><span data-stu-id="8174f-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8174f-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="8174f-182">Request</span></span>
<span data-ttu-id="8174f-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8174f-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8174f-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="8174f-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
Content-type: application/json
Content-length: 247
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": "N9917 U2883!"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category4": false
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="8174f-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8174f-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8174f-186">C#</span><span class="sxs-lookup"><span data-stu-id="8174f-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8174f-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="8174f-187">Response</span></span>
<span data-ttu-id="8174f-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8174f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1423

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
  "createdDateTime": "2015-03-24T18:36:49.2407981Z",
  "assignments": {
    "6463a5ce-2119-4198-9f2a-628761df4a62": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "N9917"
    },
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2017-04-24T22:40:44.5665917",
      "orderHint": "RWk1"
    },
    "aaa27244-1db4-476a-a5cb-004607466324": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "U2883"
    }
  },
  "appliedCategories": {
    "category3": true,
    "category5": true,
    "category6": true,
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

