# <a name="list-buckets"></a><span data-ttu-id="f738d-101">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="f738d-101">List buckets</span></span>

<span data-ttu-id="f738d-102">Получение списка объектов **plannerbucket**, содержащихся в объекте [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="f738d-102">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f738d-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f738d-103">Permissions</span></span>
<span data-ttu-id="f738d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f738d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f738d-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f738d-106">Permission type</span></span>      | <span data-ttu-id="f738d-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f738d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f738d-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f738d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f738d-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f738d-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f738d-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f738d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f738d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f738d-111">Not supported.</span></span>    |
|<span data-ttu-id="f738d-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f738d-112">Application</span></span> | <span data-ttu-id="f738d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f738d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f738d-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f738d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="f738d-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f738d-115">Request headers</span></span>
| <span data-ttu-id="f738d-116">Имя</span><span class="sxs-lookup"><span data-stu-id="f738d-116">Name</span></span>      |<span data-ttu-id="f738d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f738d-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f738d-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f738d-118">Authorization</span></span>  | <span data-ttu-id="f738d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f738d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f738d-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f738d-121">Request body</span></span>
<span data-ttu-id="f738d-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f738d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f738d-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="f738d-123">Response</span></span>

<span data-ttu-id="f738d-124">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f738d-124">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="f738d-p103">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f738d-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="f738d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f738d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f738d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f738d-129">Request</span></span>
<span data-ttu-id="f738d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f738d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="f738d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f738d-131">Response</span></span>
<span data-ttu-id="f738d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f738d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->