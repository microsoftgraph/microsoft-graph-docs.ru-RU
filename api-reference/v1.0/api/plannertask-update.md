---
title: Обновление объекта plannertask
description: Обновление свойств объекта **plannertask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8a07039166ad5ce983635980a9b901474fb4bdaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986735"
---
# <a name="update-plannertask"></a><span data-ttu-id="5659c-103">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="5659c-103">Update plannertask</span></span>

<span data-ttu-id="5659c-104">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="5659c-104">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5659c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5659c-105">Permissions</span></span>
<span data-ttu-id="5659c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5659c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5659c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5659c-108">Permission type</span></span>      | <span data-ttu-id="5659c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5659c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5659c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5659c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5659c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5659c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5659c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5659c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5659c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5659c-113">Not supported.</span></span>    |
|<span data-ttu-id="5659c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5659c-114">Application</span></span> | <span data-ttu-id="5659c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5659c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5659c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5659c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5659c-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5659c-117">Optional request headers</span></span>
| <span data-ttu-id="5659c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5659c-118">Name</span></span>       | <span data-ttu-id="5659c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5659c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5659c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5659c-120">Authorization</span></span>  | <span data-ttu-id="5659c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5659c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5659c-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="5659c-123">If-Match</span></span>  | <span data-ttu-id="5659c-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5659c-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5659c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5659c-126">Request body</span></span>
<span data-ttu-id="5659c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5659c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5659c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5659c-130">Property</span></span>     | <span data-ttu-id="5659c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5659c-131">Type</span></span>   |<span data-ttu-id="5659c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5659c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5659c-133">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="5659c-133">appliedCategories</span></span>|[<span data-ttu-id="5659c-134">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="5659c-134">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="5659c-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="5659c-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="5659c-137">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="5659c-137">assigneePriority</span></span>|<span data-ttu-id="5659c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-138">String</span></span>|<span data-ttu-id="5659c-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5659c-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5659c-141">assignments</span><span class="sxs-lookup"><span data-stu-id="5659c-141">assignments</span></span>|[<span data-ttu-id="5659c-142">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="5659c-142">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="5659c-143">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="5659c-143">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="5659c-144">bucketId</span><span class="sxs-lookup"><span data-stu-id="5659c-144">bucketId</span></span>|<span data-ttu-id="5659c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-145">String</span></span>|<span data-ttu-id="5659c-146">Код сегмента, к которой принадлежит задачи.</span><span class="sxs-lookup"><span data-stu-id="5659c-146">Bucket id to which the task belongs.</span></span> <span data-ttu-id="5659c-147">Должен быть в плане, задача находится в сегменте.</span><span class="sxs-lookup"><span data-stu-id="5659c-147">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="5659c-148">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5659c-148">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5659c-149">[Формат](../resources/planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="5659c-149">[Format validation](../resources/planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="5659c-150">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="5659c-150">conversationThreadId</span></span>|<span data-ttu-id="5659c-151">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-151">String</span></span>|<span data-ttu-id="5659c-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="5659c-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="5659c-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="5659c-154">dueDateTime</span></span>|<span data-ttu-id="5659c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5659c-155">DateTimeOffset</span></span>|<span data-ttu-id="5659c-p109">Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5659c-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5659c-159">orderHint</span><span class="sxs-lookup"><span data-stu-id="5659c-159">orderHint</span></span>|<span data-ttu-id="5659c-160">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-160">String</span></span>|<span data-ttu-id="5659c-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5659c-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5659c-163">percentComplete</span><span class="sxs-lookup"><span data-stu-id="5659c-163">percentComplete</span></span>|<span data-ttu-id="5659c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5659c-164">Int32</span></span>|<span data-ttu-id="5659c-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="5659c-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="5659c-167">planId</span><span class="sxs-lookup"><span data-stu-id="5659c-167">planId</span></span>|<span data-ttu-id="5659c-168">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-168">String</span></span>|<span data-ttu-id="5659c-169">Идентификатор плана, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="5659c-169">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="5659c-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5659c-170">startDateTime</span></span>|<span data-ttu-id="5659c-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5659c-171">DateTimeOffset</span></span>|<span data-ttu-id="5659c-p112">Дата и время начала задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5659c-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5659c-175">title</span><span class="sxs-lookup"><span data-stu-id="5659c-175">title</span></span>|<span data-ttu-id="5659c-176">Строка</span><span class="sxs-lookup"><span data-stu-id="5659c-176">String</span></span>|<span data-ttu-id="5659c-177">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="5659c-177">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="5659c-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="5659c-178">Response</span></span>

<span data-ttu-id="5659c-179">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5659c-179">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="5659c-p113">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5659c-p113">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5659c-183">Пример</span><span class="sxs-lookup"><span data-stu-id="5659c-183">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5659c-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="5659c-184">Request</span></span>
<span data-ttu-id="5659c-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5659c-185">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5659c-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="5659c-186">Response</span></span>
<span data-ttu-id="5659c-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5659c-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
