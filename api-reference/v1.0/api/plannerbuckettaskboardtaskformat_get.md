# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="e704f-101">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e704f-101">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="e704f-102">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e704f-102">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e704f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e704f-103">Permissions</span></span>
<span data-ttu-id="e704f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e704f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e704f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e704f-106">Permission type</span></span>      | <span data-ttu-id="e704f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e704f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e704f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e704f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e704f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e704f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e704f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e704f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e704f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e704f-111">Not supported.</span></span>    |
|<span data-ttu-id="e704f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e704f-112">Application</span></span> | <span data-ttu-id="e704f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e704f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e704f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e704f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="e704f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e704f-115">Request headers</span></span>
| <span data-ttu-id="e704f-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e704f-116">Name</span></span>      |<span data-ttu-id="e704f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e704f-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e704f-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e704f-118">Authorization</span></span>  | <span data-ttu-id="e704f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e704f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e704f-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e704f-121">Request body</span></span>
<span data-ttu-id="e704f-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e704f-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e704f-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="e704f-123">Response</span></span>

<span data-ttu-id="e704f-124">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e704f-124">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e704f-p103">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e704f-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e704f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e704f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e704f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e704f-129">Request</span></span>
<span data-ttu-id="e704f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e704f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="e704f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e704f-131">Response</span></span>
<span data-ttu-id="e704f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e704f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->