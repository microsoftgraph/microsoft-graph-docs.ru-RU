---
title: Обновление объекта plannertask
description: Обновление свойств объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a0973fccf01a7f631e075cd6c4d3383b46613048
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049984"
---
# <a name="update-plannertask"></a><span data-ttu-id="49890-103">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="49890-103">Update plannertask</span></span>

<span data-ttu-id="49890-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49890-105">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="49890-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49890-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49890-106">Permissions</span></span>
<span data-ttu-id="49890-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49890-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49890-109">Permission type</span></span>      | <span data-ttu-id="49890-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49890-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49890-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49890-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49890-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49890-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49890-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49890-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49890-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49890-114">Not supported.</span></span>    |
|<span data-ttu-id="49890-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49890-115">Application</span></span> | <span data-ttu-id="49890-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49890-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49890-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49890-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="49890-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49890-118">Optional request headers</span></span>
| <span data-ttu-id="49890-119">Имя</span><span class="sxs-lookup"><span data-stu-id="49890-119">Name</span></span>       | <span data-ttu-id="49890-120">Описание</span><span class="sxs-lookup"><span data-stu-id="49890-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="49890-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49890-121">Authorization</span></span>  | <span data-ttu-id="49890-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49890-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49890-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="49890-124">If-Match</span></span>  | <span data-ttu-id="49890-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49890-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49890-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49890-127">Request body</span></span>
<span data-ttu-id="49890-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="49890-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="49890-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="49890-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="49890-130">Для лучшей производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="49890-130">For best performance,  don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="49890-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="49890-131">Property</span></span>     | <span data-ttu-id="49890-132">Тип</span><span class="sxs-lookup"><span data-stu-id="49890-132">Type</span></span>   |<span data-ttu-id="49890-133">Описание</span><span class="sxs-lookup"><span data-stu-id="49890-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49890-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="49890-134">appliedCategories</span></span>|[<span data-ttu-id="49890-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="49890-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="49890-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="49890-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="49890-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="49890-138">assigneePriority</span></span>|<span data-ttu-id="49890-139">String</span><span class="sxs-lookup"><span data-stu-id="49890-139">String</span></span>|<span data-ttu-id="49890-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="49890-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="49890-142">assignments</span><span class="sxs-lookup"><span data-stu-id="49890-142">assignments</span></span>|[<span data-ttu-id="49890-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="49890-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="49890-144">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="49890-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="49890-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="49890-145">bucketId</span></span>|<span data-ttu-id="49890-146">Строка</span><span class="sxs-lookup"><span data-stu-id="49890-146">String</span></span>|<span data-ttu-id="49890-147">Ведерный id, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="49890-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="49890-148">Сегмент должен находиться в том же плане, что и задача.</span><span class="sxs-lookup"><span data-stu-id="49890-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="49890-149">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="49890-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="49890-150">[Проверка формата](../resources/tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="49890-150">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="49890-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="49890-151">conversationThreadId</span></span>|<span data-ttu-id="49890-152">Строка</span><span class="sxs-lookup"><span data-stu-id="49890-152">String</span></span>|<span data-ttu-id="49890-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="49890-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="49890-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="49890-155">dueDateTime</span></span>|<span data-ttu-id="49890-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49890-156">DateTimeOffset</span></span>|<span data-ttu-id="49890-157">Срок выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="49890-157">Date and time at which the task is due.</span></span> <span data-ttu-id="49890-158">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="49890-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49890-159">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="49890-159">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="49890-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="49890-160">orderHint</span></span>|<span data-ttu-id="49890-161">String</span><span class="sxs-lookup"><span data-stu-id="49890-161">String</span></span>|<span data-ttu-id="49890-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="49890-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="49890-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="49890-164">percentComplete</span></span>|<span data-ttu-id="49890-165">Int32</span><span class="sxs-lookup"><span data-stu-id="49890-165">Int32</span></span>|<span data-ttu-id="49890-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="49890-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="49890-168">planId</span><span class="sxs-lookup"><span data-stu-id="49890-168">planId</span></span>|<span data-ttu-id="49890-169">Строка</span><span class="sxs-lookup"><span data-stu-id="49890-169">String</span></span>|<span data-ttu-id="49890-170">Идентификатор плана, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="49890-170">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="49890-171">priority</span><span class="sxs-lookup"><span data-stu-id="49890-171">priority</span></span>|<span data-ttu-id="49890-172">Int32</span><span class="sxs-lookup"><span data-stu-id="49890-172">Int32</span></span>|<span data-ttu-id="49890-173">Приоритет задачи.</span><span class="sxs-lookup"><span data-stu-id="49890-173">Priority of the task.</span></span> <span data-ttu-id="49890-174">Допустимый диапазон значений находится между и (включительно), при этом увеличение значения является более низким приоритетом (имеет самый высокий приоритет и имеет самый `0` `10` низкий `0` `10` приоритет).</span><span class="sxs-lookup"><span data-stu-id="49890-174">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="49890-175">В настоящее время Planner интерпретирует значения и как `0` `1` "срочные", и как `2` `3` `4` "важные", и как "средний", и , и , и `5` `6` как `7` `8` `9` `10` "низкий".</span><span class="sxs-lookup"><span data-stu-id="49890-175">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="49890-176">В настоящее время планировщик задает значение `1` "urgent", `3` "important", `5` "medium" и `9` "low".</span><span class="sxs-lookup"><span data-stu-id="49890-176">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="49890-177">startDateTime</span><span class="sxs-lookup"><span data-stu-id="49890-177">startDateTime</span></span>|<span data-ttu-id="49890-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49890-178">DateTimeOffset</span></span>|<span data-ttu-id="49890-179">Дата и время начала задачи.</span><span class="sxs-lookup"><span data-stu-id="49890-179">Date and time at which the task starts.</span></span> <span data-ttu-id="49890-180">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="49890-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49890-181">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="49890-181">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="49890-182">title</span><span class="sxs-lookup"><span data-stu-id="49890-182">title</span></span>|<span data-ttu-id="49890-183">Строка</span><span class="sxs-lookup"><span data-stu-id="49890-183">String</span></span>|<span data-ttu-id="49890-184">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="49890-184">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="49890-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="49890-185">Response</span></span>

<span data-ttu-id="49890-186">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="49890-186">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="49890-187">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный `Prefer` `return=representation` объект `200 OK` [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49890-187">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="49890-p115">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="49890-p115">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="49890-191">Пример</span><span class="sxs-lookup"><span data-stu-id="49890-191">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49890-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="49890-192">Request</span></span>
<span data-ttu-id="49890-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49890-193">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49890-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="49890-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
Content-type: application/json
Content-length: 247
Prefer: return=representation
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
# <a name="javascript"></a>[<span data-ttu-id="49890-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49890-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="49890-196">C#</span><span class="sxs-lookup"><span data-stu-id="49890-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49890-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="49890-197">Response</span></span>
<span data-ttu-id="49890-198">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49890-198">Here is an example of the response.</span></span> 

><span data-ttu-id="49890-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49890-199">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


