# <a name="update-plannertask"></a><span data-ttu-id="a7dbf-101">Обновление объекта plannertask</span><span class="sxs-lookup"><span data-stu-id="a7dbf-101">Update plannertask</span></span>

<span data-ttu-id="a7dbf-102">Обновление свойств объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-102">Update the properties of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7dbf-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dbf-103">Permissions</span></span>
<span data-ttu-id="a7dbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7dbf-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dbf-106">Permission type</span></span>      | <span data-ttu-id="a7dbf-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7dbf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7dbf-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7dbf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a7dbf-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7dbf-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7dbf-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7dbf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7dbf-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-111">Not supported.</span></span>    |
|<span data-ttu-id="a7dbf-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7dbf-112">Application</span></span> | <span data-ttu-id="a7dbf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7dbf-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7dbf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="a7dbf-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7dbf-115">Optional request headers</span></span>
| <span data-ttu-id="a7dbf-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a7dbf-116">Name</span></span>       | <span data-ttu-id="a7dbf-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dbf-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a7dbf-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7dbf-118">Authorization</span></span>  | <span data-ttu-id="a7dbf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7dbf-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="a7dbf-121">If-Match</span></span>  | <span data-ttu-id="a7dbf-p103">Последнее известное значение ETag обновляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p103">Last known ETag value for the **plannerTask** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7dbf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7dbf-124">Request body</span></span>
<span data-ttu-id="a7dbf-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7dbf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7dbf-128">Property</span></span>     | <span data-ttu-id="a7dbf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a7dbf-129">Type</span></span>   |<span data-ttu-id="a7dbf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dbf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7dbf-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="a7dbf-131">appliedCategories</span></span>|[<span data-ttu-id="a7dbf-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="a7dbf-132">plannerAppliedCategories</span></span>](../resources/plannerappliedcategories.md)|<span data-ttu-id="a7dbf-p105">Категории, к которым применена задача. Возможные значения см. [здесь](../resources/plannerappliedcategories.md).</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p105">The categories to which the task has been applied. See [applied Categories](../resources/plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="a7dbf-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="a7dbf-135">assigneePriority</span></span>|<span data-ttu-id="a7dbf-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a7dbf-136">String</span></span>|<span data-ttu-id="a7dbf-p106">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p106">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="a7dbf-139">assignments</span><span class="sxs-lookup"><span data-stu-id="a7dbf-139">assignments</span></span>|[<span data-ttu-id="a7dbf-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="a7dbf-140">plannerAssignments</span></span>](../resources/plannerassignments.md)|<span data-ttu-id="a7dbf-141">Список пользователей, которым назначена задача.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-141">The set of users the task is assigned to.</span></span>|
|<span data-ttu-id="a7dbf-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="a7dbf-142">bucketId</span></span>|<span data-ttu-id="a7dbf-143">String</span><span class="sxs-lookup"><span data-stu-id="a7dbf-143">String</span></span>|<span data-ttu-id="a7dbf-p107">Идентификатор сегмента, к которому относится задача. Сегмент должен находиться в том же плане, что и задача. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](../resources/planner_identifiers_disclaimer.md) проводится для службе.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p107">Bucket id to which the task belongs. The bucket needs to be in the plan that the task is in. It is 28 characters long and case sensitive. [Format validation](../resources/planner_identifiers_disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="a7dbf-148">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="a7dbf-148">conversationThreadId</span></span>|<span data-ttu-id="a7dbf-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a7dbf-149">String</span></span>|<span data-ttu-id="a7dbf-p108">Идентификатор беседы в задаче. Это идентификатор объекта беседы, созданной в группе.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p108">Thread id of the conversation on the task. This is the id of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="a7dbf-152">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a7dbf-152">dueDateTime</span></span>|<span data-ttu-id="a7dbf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7dbf-153">DateTimeOffset</span></span>|<span data-ttu-id="a7dbf-p109">Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a7dbf-157">orderHint</span><span class="sxs-lookup"><span data-stu-id="a7dbf-157">orderHint</span></span>|<span data-ttu-id="a7dbf-158">String</span><span class="sxs-lookup"><span data-stu-id="a7dbf-158">String</span></span>|<span data-ttu-id="a7dbf-p110">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p110">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="a7dbf-161">percentComplete</span><span class="sxs-lookup"><span data-stu-id="a7dbf-161">percentComplete</span></span>|<span data-ttu-id="a7dbf-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a7dbf-162">Int32</span></span>|<span data-ttu-id="a7dbf-p111">Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p111">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="a7dbf-165">planId</span><span class="sxs-lookup"><span data-stu-id="a7dbf-165">planId</span></span>|<span data-ttu-id="a7dbf-166">Строка</span><span class="sxs-lookup"><span data-stu-id="a7dbf-166">String</span></span>|<span data-ttu-id="a7dbf-167">Идентификатор плана, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-167">Plan id to which the task belongs.</span></span>|
|<span data-ttu-id="a7dbf-168">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7dbf-168">startDateTime</span></span>|<span data-ttu-id="a7dbf-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7dbf-169">DateTimeOffset</span></span>|<span data-ttu-id="a7dbf-p112">Дата и время начала задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p112">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a7dbf-173">title</span><span class="sxs-lookup"><span data-stu-id="a7dbf-173">title</span></span>|<span data-ttu-id="a7dbf-174">Строка</span><span class="sxs-lookup"><span data-stu-id="a7dbf-174">String</span></span>|<span data-ttu-id="a7dbf-175">Название задачи.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-175">Title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="a7dbf-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7dbf-176">Response</span></span>

<span data-ttu-id="a7dbf-177">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-177">If successful, this method returns a `200 OK` response code and updated [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="a7dbf-p113">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p113">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a7dbf-181">Пример</span><span class="sxs-lookup"><span data-stu-id="a7dbf-181">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7dbf-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7dbf-182">Request</span></span>
<span data-ttu-id="a7dbf-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-183">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
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
##### <a name="response"></a><span data-ttu-id="a7dbf-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7dbf-184">Response</span></span>
<span data-ttu-id="a7dbf-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7dbf-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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