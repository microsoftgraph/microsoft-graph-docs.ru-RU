# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="6398c-101">Обновление объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6398c-101">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="6398c-102">Обновление свойств объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="6398c-102">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6398c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6398c-103">Permissions</span></span>
<span data-ttu-id="6398c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6398c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6398c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6398c-106">Permission type</span></span>      | <span data-ttu-id="6398c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6398c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6398c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6398c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6398c-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6398c-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6398c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6398c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6398c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6398c-111">Not supported.</span></span>    |
|<span data-ttu-id="6398c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6398c-112">Application</span></span> | <span data-ttu-id="6398c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6398c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6398c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6398c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="6398c-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6398c-115">Optional request headers</span></span>
| <span data-ttu-id="6398c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="6398c-116">Name</span></span>       | <span data-ttu-id="6398c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6398c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6398c-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6398c-118">Authorization</span></span>  | <span data-ttu-id="6398c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6398c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6398c-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="6398c-121">If-Match</span></span>  | <span data-ttu-id="6398c-p103">Последнее известное значение ETag обновляемого объекта **plannerAssignedToTaskBoardTaskFormat**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6398c-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6398c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6398c-124">Request body</span></span>
<span data-ttu-id="6398c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6398c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6398c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6398c-128">Property</span></span>     | <span data-ttu-id="6398c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6398c-129">Type</span></span>   |<span data-ttu-id="6398c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6398c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6398c-131">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="6398c-131">orderHintsByAssignee</span></span>|[<span data-ttu-id="6398c-132">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="6398c-132">plannerOrderHintsByAssignee</span></span>](..\resources\plannerOrderHintsByAssignee.md)|<span data-ttu-id="6398c-p105">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="6398c-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="6398c-136">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="6398c-136">unassignedOrderHint</span></span>|<span data-ttu-id="6398c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6398c-137">String</span></span>|<span data-ttu-id="6398c-p106">Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="6398c-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="6398c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6398c-140">Response</span></span>

<span data-ttu-id="6398c-141">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6398c-141">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="6398c-p107">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6398c-p107">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6398c-145">Пример</span><span class="sxs-lookup"><span data-stu-id="6398c-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6398c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6398c-146">Request</span></span>
<span data-ttu-id="6398c-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6398c-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a><span data-ttu-id="6398c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="6398c-148">Response</span></span>
<span data-ttu-id="6398c-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6398c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->