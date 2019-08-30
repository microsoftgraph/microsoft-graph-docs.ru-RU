---
title: Обновление объекта plannertask
description: Обновление свойств объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 982457fde0bdd4cb4d5b1305642de5cf3faf6185
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677185"
---
# <a name="update-plannertask"></a><span data-ttu-id="e5f21-103">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="e5f21-103">Update plannertask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5f21-104">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="e5f21-104">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5f21-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f21-105">Permissions</span></span>
<span data-ttu-id="e5f21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5f21-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f21-108">Permission type</span></span>      | <span data-ttu-id="e5f21-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5f21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5f21-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5f21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5f21-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5f21-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5f21-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5f21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5f21-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5f21-113">Not supported.</span></span>    |
|<span data-ttu-id="e5f21-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5f21-114">Application</span></span> | <span data-ttu-id="e5f21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5f21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5f21-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5f21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e5f21-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5f21-117">Optional request headers</span></span>
| <span data-ttu-id="e5f21-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5f21-118">Name</span></span>       | <span data-ttu-id="e5f21-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f21-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e5f21-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5f21-120">Authorization</span></span>  | <span data-ttu-id="e5f21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5f21-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="e5f21-123">If-Match</span></span>  | <span data-ttu-id="e5f21-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5f21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5f21-126">Request body</span></span>
<span data-ttu-id="e5f21-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e5f21-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e5f21-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e5f21-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e5f21-129">Для достижения лучшей производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e5f21-129">For best performance,  don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5f21-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5f21-130">Property</span></span>     | <span data-ttu-id="e5f21-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5f21-131">Type</span></span>   |<span data-ttu-id="e5f21-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f21-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5f21-133">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="e5f21-133">appliedCategories</span></span>|[<span data-ttu-id="e5f21-134">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="e5f21-134">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="e5f21-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="e5f21-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="e5f21-137">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="e5f21-137">assigneePriority</span></span>|<span data-ttu-id="e5f21-138">String</span><span class="sxs-lookup"><span data-stu-id="e5f21-138">String</span></span>|<span data-ttu-id="e5f21-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e5f21-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e5f21-141">assignments</span><span class="sxs-lookup"><span data-stu-id="e5f21-141">assignments</span></span>|[<span data-ttu-id="e5f21-142">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="e5f21-142">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="e5f21-143">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="e5f21-143">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="e5f21-144">bucketId</span><span class="sxs-lookup"><span data-stu-id="e5f21-144">bucketId</span></span>|<span data-ttu-id="e5f21-145">String</span><span class="sxs-lookup"><span data-stu-id="e5f21-145">String</span></span>|<span data-ttu-id="e5f21-146">Идентификатор контейнера, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="e5f21-146">Bucket id to which the task belongs.</span></span> <span data-ttu-id="e5f21-147">Сегмент должен находиться в том же плане, что и задача.</span><span class="sxs-lookup"><span data-stu-id="e5f21-147">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="e5f21-148">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e5f21-148">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e5f21-149">[Проверка формата](../resources/tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="e5f21-149">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="e5f21-150">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="e5f21-150">conversationThreadId</span></span>|<span data-ttu-id="e5f21-151">String</span><span class="sxs-lookup"><span data-stu-id="e5f21-151">String</span></span>|<span data-ttu-id="e5f21-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="e5f21-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f21-154">dueDateTime</span></span>|<span data-ttu-id="e5f21-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f21-155">DateTimeOffset</span></span>|<span data-ttu-id="e5f21-p109">Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e5f21-159">orderHint</span><span class="sxs-lookup"><span data-stu-id="e5f21-159">orderHint</span></span>|<span data-ttu-id="e5f21-160">String</span><span class="sxs-lookup"><span data-stu-id="e5f21-160">String</span></span>|<span data-ttu-id="e5f21-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e5f21-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e5f21-163">percentComplete</span><span class="sxs-lookup"><span data-stu-id="e5f21-163">percentComplete</span></span>|<span data-ttu-id="e5f21-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e5f21-164">Int32</span></span>|<span data-ttu-id="e5f21-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="e5f21-167">priority</span><span class="sxs-lookup"><span data-stu-id="e5f21-167">priority</span></span>|<span data-ttu-id="e5f21-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e5f21-168">Int32</span></span>|<span data-ttu-id="e5f21-169">Приоритет задачи.</span><span class="sxs-lookup"><span data-stu-id="e5f21-169">Priority of the task.</span></span> <span data-ttu-id="e5f21-170">Допустимый диапазон значений: между `0` и `10` (включительно), при котором увеличивается значение низкого приоритета (`0` имеет самый высокий `10` приоритет и имеет самый низкий приоритет).</span><span class="sxs-lookup"><span data-stu-id="e5f21-170">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="e5f21-171">В настоящее время планировщик интерпретирует значения `0` , `1` а также как "срочные `3` " `4` , `2` а также `5` `6` `7` "средний", "средний" и "средний" `8`, `9` `10` а также "средний".</span><span class="sxs-lookup"><span data-stu-id="e5f21-171">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="e5f21-172">В настоящее время планировщик устанавливает значение `1` "срочно", `3` "важно" `5` , "среднее" и `9` "недорогой".</span><span class="sxs-lookup"><span data-stu-id="e5f21-172">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="e5f21-173">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f21-173">startDateTime</span></span>|<span data-ttu-id="e5f21-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f21-174">DateTimeOffset</span></span>|<span data-ttu-id="e5f21-p113">Дата и время начала задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e5f21-178">title</span><span class="sxs-lookup"><span data-stu-id="e5f21-178">title</span></span>|<span data-ttu-id="e5f21-179">Строка</span><span class="sxs-lookup"><span data-stu-id="e5f21-179">String</span></span>|<span data-ttu-id="e5f21-180">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="e5f21-180">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="e5f21-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5f21-181">Response</span></span>

<span data-ttu-id="e5f21-182">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerTask](../resources/plannertask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5f21-182">If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="e5f21-p114">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e5f21-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e5f21-186">Пример</span><span class="sxs-lookup"><span data-stu-id="e5f21-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5f21-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5f21-187">Request</span></span>
<span data-ttu-id="e5f21-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5f21-188">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5f21-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5f21-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5f21-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5f21-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5f21-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5f21-191">Response</span></span>
<span data-ttu-id="e5f21-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5f21-192">Here is an example of the response.</span></span> 

><span data-ttu-id="e5f21-p115">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5f21-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
