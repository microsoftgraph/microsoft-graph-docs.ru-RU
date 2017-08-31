# <a name="update-plannerbucket"></a><span data-ttu-id="b2fb3-101">Обновление объекта plannerbucket</span><span class="sxs-lookup"><span data-stu-id="b2fb3-101">Update plannerbucket</span></span>

<span data-ttu-id="b2fb3-102">Обновление свойств объекта **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-102">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2fb3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2fb3-103">Permissions</span></span>
<span data-ttu-id="b2fb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2fb3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2fb3-106">Permission type</span></span>      | <span data-ttu-id="b2fb3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2fb3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2fb3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2fb3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b2fb3-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fb3-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2fb3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2fb3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2fb3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-111">Not supported.</span></span>    |
|<span data-ttu-id="b2fb3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2fb3-112">Application</span></span> | <span data-ttu-id="b2fb3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2fb3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2fb3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="b2fb3-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2fb3-115">Optional request headers</span></span>
| <span data-ttu-id="b2fb3-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b2fb3-116">Name</span></span>       | <span data-ttu-id="b2fb3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="b2fb3-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b2fb3-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2fb3-118">Authorization</span></span>  | <span data-ttu-id="b2fb3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2fb3-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="b2fb3-121">If-Match</span></span>  | <span data-ttu-id="b2fb3-p103">Последнее известное значение ETag обновляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2fb3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2fb3-124">Request body</span></span>
<span data-ttu-id="b2fb3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b2fb3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2fb3-128">Property</span></span>     | <span data-ttu-id="b2fb3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b2fb3-129">Type</span></span>   |<span data-ttu-id="b2fb3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b2fb3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2fb3-131">name</span><span class="sxs-lookup"><span data-stu-id="b2fb3-131">name</span></span>|<span data-ttu-id="b2fb3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b2fb3-132">String</span></span>|<span data-ttu-id="b2fb3-133">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-133">Name of the bucket.</span></span>|
|<span data-ttu-id="b2fb3-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="b2fb3-134">orderHint</span></span>|<span data-ttu-id="b2fb3-135">String</span><span class="sxs-lookup"><span data-stu-id="b2fb3-135">String</span></span>|<span data-ttu-id="b2fb3-p105">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](../resources/planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="b2fb3-138">planId</span><span class="sxs-lookup"><span data-stu-id="b2fb3-138">planId</span></span>|<span data-ttu-id="b2fb3-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b2fb3-139">String</span></span>|<span data-ttu-id="b2fb3-140">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-140">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="b2fb3-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2fb3-141">Response</span></span>

<span data-ttu-id="b2fb3-142">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-142">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="b2fb3-p106">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b2fb3-146">Пример</span><span class="sxs-lookup"><span data-stu-id="b2fb3-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2fb3-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2fb3-147">Request</span></span>
<span data-ttu-id="b2fb3-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="b2fb3-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2fb3-149">Response</span></span>
<span data-ttu-id="b2fb3-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2fb3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->