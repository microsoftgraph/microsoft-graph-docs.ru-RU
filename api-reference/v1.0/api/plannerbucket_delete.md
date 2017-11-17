# <a name="delete-plannerbucket"></a><span data-ttu-id="a124a-101">Удаление объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="a124a-101">Delete plannerBucket</span></span>

<span data-ttu-id="a124a-102">Удаление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="a124a-102">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="a124a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a124a-103">Permissions</span></span>
<span data-ttu-id="a124a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a124a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a124a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a124a-106">Permission type</span></span>      | <span data-ttu-id="a124a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a124a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a124a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a124a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a124a-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a124a-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a124a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a124a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a124a-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a124a-111">Not supported.</span></span>    |
|<span data-ttu-id="a124a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a124a-112">Application</span></span> | <span data-ttu-id="a124a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a124a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a124a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a124a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/<id>
```
## <a name="request-headers"></a><span data-ttu-id="a124a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a124a-115">Request headers</span></span>
| <span data-ttu-id="a124a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a124a-116">Name</span></span>       | <span data-ttu-id="a124a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a124a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a124a-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a124a-118">Authorization</span></span>  | <span data-ttu-id="a124a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a124a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a124a-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="a124a-121">If-Match</span></span>  | <span data-ttu-id="a124a-p103">Последнее известное значение ETag удаляемого объекта **plannerBucket**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a124a-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a124a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a124a-124">Request body</span></span>
<span data-ttu-id="a124a-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a124a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a124a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a124a-126">Response</span></span>

<span data-ttu-id="a124a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a124a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="a124a-p105">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a124a-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a124a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a124a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a124a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a124a-133">Request</span></span>
<span data-ttu-id="a124a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a124a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/buckets/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="a124a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a124a-135">Response</span></span>
<span data-ttu-id="a124a-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a124a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->