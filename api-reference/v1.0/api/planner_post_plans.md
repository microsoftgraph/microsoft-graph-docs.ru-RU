# <a name="create-plannerplan"></a><span data-ttu-id="7ea39-101">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7ea39-101">Create plannerPlan</span></span>

<span data-ttu-id="7ea39-102">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="7ea39-102">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ea39-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ea39-103">Permissions</span></span>
<span data-ttu-id="7ea39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ea39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7ea39-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ea39-106">Permission type</span></span>      | <span data-ttu-id="7ea39-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ea39-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ea39-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ea39-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7ea39-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ea39-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ea39-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ea39-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ea39-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ea39-111">Not supported.</span></span>    |
|<span data-ttu-id="7ea39-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ea39-112">Application</span></span> | <span data-ttu-id="7ea39-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ea39-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ea39-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ea39-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/plans

```
## <a name="request-headers"></a><span data-ttu-id="7ea39-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ea39-115">Request headers</span></span>
| <span data-ttu-id="7ea39-116">Имя</span><span class="sxs-lookup"><span data-stu-id="7ea39-116">Name</span></span>       | <span data-ttu-id="7ea39-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7ea39-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ea39-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ea39-118">Authorization</span></span>  | <span data-ttu-id="7ea39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ea39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ea39-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ea39-121">Request body</span></span>
<span data-ttu-id="7ea39-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7ea39-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7ea39-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ea39-124">Response</span></span>

<span data-ttu-id="7ea39-125">В случае успеха этот метод возвращает код ответа `201, Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7ea39-125">If successful, this method returns `201, Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="7ea39-p104">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7ea39-p104">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7ea39-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7ea39-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ea39-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ea39-130">Request</span></span>
<span data-ttu-id="7ea39-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ea39-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
<span data-ttu-id="7ea39-132">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ea39-132">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7ea39-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ea39-133">Response</span></span>
<span data-ttu-id="7ea39-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ea39-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->