# <a name="get-plannerplan"></a><span data-ttu-id="21c2e-101">Получение объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="21c2e-101">Get plannerPlan</span></span>

<span data-ttu-id="21c2e-102">Получение свойств и связей объекта **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="21c2e-102">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21c2e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21c2e-103">Permissions</span></span>
<span data-ttu-id="21c2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="21c2e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21c2e-106">Permission type</span></span>      | <span data-ttu-id="21c2e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21c2e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21c2e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21c2e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="21c2e-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21c2e-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21c2e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21c2e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21c2e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21c2e-111">Not supported.</span></span>    |
|<span data-ttu-id="21c2e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21c2e-112">Application</span></span> | <span data-ttu-id="21c2e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21c2e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21c2e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21c2e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="21c2e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21c2e-115">Request headers</span></span>
| <span data-ttu-id="21c2e-116">Имя</span><span class="sxs-lookup"><span data-stu-id="21c2e-116">Name</span></span>      |<span data-ttu-id="21c2e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="21c2e-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21c2e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21c2e-118">Authorization</span></span>  | <span data-ttu-id="21c2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21c2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21c2e-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21c2e-121">Request body</span></span>
<span data-ttu-id="21c2e-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21c2e-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21c2e-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="21c2e-123">Response</span></span>

<span data-ttu-id="21c2e-124">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21c2e-124">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="21c2e-p103">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="21c2e-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="21c2e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="21c2e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21c2e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="21c2e-129">Request</span></span>
<span data-ttu-id="21c2e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21c2e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM
```
##### <a name="response"></a><span data-ttu-id="21c2e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="21c2e-131">Response</span></span>
<span data-ttu-id="21c2e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21c2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->