---
title: Обновление объекта plannertask
description: Обновление свойств объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 955412f1f699f374b974cfdde81c8baedc4021dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095816"
---
# <a name="update-plannertask"></a><span data-ttu-id="f52f0-103">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="f52f0-103">Update plannertask</span></span>

<span data-ttu-id="f52f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f52f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f52f0-105">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="f52f0-105">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f52f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f52f0-106">Permissions</span></span>
<span data-ttu-id="f52f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f52f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f52f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f52f0-109">Permission type</span></span>      | <span data-ttu-id="f52f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f52f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f52f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f52f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f52f0-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f52f0-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f52f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f52f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f52f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f52f0-114">Not supported.</span></span>    |
|<span data-ttu-id="f52f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f52f0-115">Application</span></span> | <span data-ttu-id="f52f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f52f0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f52f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f52f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f52f0-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f52f0-118">Optional request headers</span></span>
| <span data-ttu-id="f52f0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f52f0-119">Name</span></span>       | <span data-ttu-id="f52f0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f52f0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f52f0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f52f0-121">Authorization</span></span>  | <span data-ttu-id="f52f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f52f0-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="f52f0-124">If-Match</span></span>  | <span data-ttu-id="f52f0-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f52f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f52f0-127">Request body</span></span>
<span data-ttu-id="f52f0-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f52f0-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f52f0-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f52f0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f52f0-130">Для достижения лучшей производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f52f0-130">For best performance,  don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f52f0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f52f0-131">Property</span></span>     | <span data-ttu-id="f52f0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f52f0-132">Type</span></span>   |<span data-ttu-id="f52f0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f52f0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f52f0-134">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="f52f0-134">appliedCategories</span></span>|[<span data-ttu-id="f52f0-135">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="f52f0-135">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="f52f0-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="f52f0-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="f52f0-138">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="f52f0-138">assigneePriority</span></span>|<span data-ttu-id="f52f0-139">String</span><span class="sxs-lookup"><span data-stu-id="f52f0-139">String</span></span>|<span data-ttu-id="f52f0-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f52f0-p106">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f52f0-142">assignments</span><span class="sxs-lookup"><span data-stu-id="f52f0-142">assignments</span></span>|[<span data-ttu-id="f52f0-143">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="f52f0-143">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="f52f0-144">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="f52f0-144">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="f52f0-145">bucketId</span><span class="sxs-lookup"><span data-stu-id="f52f0-145">bucketId</span></span>|<span data-ttu-id="f52f0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f52f0-146">String</span></span>|<span data-ttu-id="f52f0-147">Идентификатор контейнера, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="f52f0-147">Bucket id to which the task belongs.</span></span> <span data-ttu-id="f52f0-148">Сегмент должен находиться в том же плане, что и задача.</span><span class="sxs-lookup"><span data-stu-id="f52f0-148">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="f52f0-149">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f52f0-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f52f0-150">[Проверка формата](../resources/tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="f52f0-150">[Format validation](../resources/tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="f52f0-151">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="f52f0-151">conversationThreadId</span></span>|<span data-ttu-id="f52f0-152">Строка</span><span class="sxs-lookup"><span data-stu-id="f52f0-152">String</span></span>|<span data-ttu-id="f52f0-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="f52f0-155">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="f52f0-155">dueDateTime</span></span>|<span data-ttu-id="f52f0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f52f0-156">DateTimeOffset</span></span>|<span data-ttu-id="f52f0-p109">Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f52f0-160">orderHint</span><span class="sxs-lookup"><span data-stu-id="f52f0-160">orderHint</span></span>|<span data-ttu-id="f52f0-161">String</span><span class="sxs-lookup"><span data-stu-id="f52f0-161">String</span></span>|<span data-ttu-id="f52f0-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f52f0-p110">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f52f0-164">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f52f0-164">percentComplete</span></span>|<span data-ttu-id="f52f0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f52f0-165">Int32</span></span>|<span data-ttu-id="f52f0-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="f52f0-168">priority</span><span class="sxs-lookup"><span data-stu-id="f52f0-168">priority</span></span>|<span data-ttu-id="f52f0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f52f0-169">Int32</span></span>|<span data-ttu-id="f52f0-170">Приоритет задачи.</span><span class="sxs-lookup"><span data-stu-id="f52f0-170">Priority of the task.</span></span> <span data-ttu-id="f52f0-171">Допустимый диапазон значений: между `0` и `10` (включительно), при котором увеличивается значение низкого приоритета ( `0` имеет самый высокий приоритет и `10` имеет самый низкий приоритет).</span><span class="sxs-lookup"><span data-stu-id="f52f0-171">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="f52f0-172">В настоящее время планировщик интерпретирует значения `0` , а также как " `1` срочные", а также "средний", " `2` `3` средний" и " `4` `5` `6` `7` средний", а также "средний" `8` `9` `10` .</span><span class="sxs-lookup"><span data-stu-id="f52f0-172">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="f52f0-173">В настоящее время планировщик устанавливает значение `1` "срочно", " `3` важно", `5` "среднее" и `9` "недорогой".</span><span class="sxs-lookup"><span data-stu-id="f52f0-173">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="f52f0-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f52f0-174">startDateTime</span></span>|<span data-ttu-id="f52f0-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f52f0-175">DateTimeOffset</span></span>|<span data-ttu-id="f52f0-p113">Дата и время начала задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p113">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f52f0-179">title</span><span class="sxs-lookup"><span data-stu-id="f52f0-179">title</span></span>|<span data-ttu-id="f52f0-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f52f0-180">String</span></span>|<span data-ttu-id="f52f0-181">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="f52f0-181">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="f52f0-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="f52f0-182">Response</span></span>

<span data-ttu-id="f52f0-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerTask](../resources/plannertask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f52f0-183">If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="f52f0-p114">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f52f0-p114">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f52f0-187">Пример</span><span class="sxs-lookup"><span data-stu-id="f52f0-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f52f0-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="f52f0-188">Request</span></span>
<span data-ttu-id="f52f0-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f52f0-189">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f52f0-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="f52f0-190">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="f52f0-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f52f0-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f52f0-192">C#</span><span class="sxs-lookup"><span data-stu-id="f52f0-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52f0-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="f52f0-193">Response</span></span>
<span data-ttu-id="f52f0-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f52f0-194">Here is an example of the response.</span></span> 

><span data-ttu-id="f52f0-p115">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f52f0-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


