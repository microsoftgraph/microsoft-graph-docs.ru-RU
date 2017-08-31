# <a name="get-plannertask"></a><span data-ttu-id="7b0e9-101">Получение объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="7b0e9-101">Get plannerTask</span></span>

<span data-ttu-id="7b0e9-102">Получение свойств и связей объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-102">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b0e9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b0e9-103">Permissions</span></span>
<span data-ttu-id="7b0e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b0e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b0e9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b0e9-106">Permission type</span></span>      | <span data-ttu-id="7b0e9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b0e9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b0e9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b0e9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7b0e9-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b0e9-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b0e9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b0e9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b0e9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-111">Not supported.</span></span>    |
|<span data-ttu-id="7b0e9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b0e9-112">Application</span></span> | <span data-ttu-id="7b0e9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b0e9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b0e9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>
```

## <a name="request-headers"></a><span data-ttu-id="7b0e9-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b0e9-115">Request headers</span></span>
| <span data-ttu-id="7b0e9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="7b0e9-116">Name</span></span>      |<span data-ttu-id="7b0e9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7b0e9-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b0e9-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b0e9-118">Authorization</span></span>  | <span data-ttu-id="7b0e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b0e9-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b0e9-121">Request body</span></span>
<span data-ttu-id="7b0e9-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b0e9-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b0e9-123">Response</span></span>

<span data-ttu-id="7b0e9-124">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-124">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="7b0e9-p103">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7b0e9-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7b0e9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7b0e9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b0e9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b0e9-129">Request</span></span>
<span data-ttu-id="7b0e9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh
```
##### <a name="response"></a><span data-ttu-id="7b0e9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b0e9-131">Response</span></span>
<span data-ttu-id="7b0e9-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b0e9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

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
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
        }
      },
      "assignedDateTime": "2015-03-25T18:38:21.956Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->