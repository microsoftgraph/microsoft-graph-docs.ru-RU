# <a name="create-plannerplan"></a><span data-ttu-id="a8360-101">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a8360-101">Create plannerPlan</span></span>

<span data-ttu-id="a8360-102">Используйте этот API, чтобы создать объект **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="a8360-102">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8360-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8360-103">Permissions</span></span>

<span data-ttu-id="a8360-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a8360-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8360-106">Permission type</span></span>                        | <span data-ttu-id="a8360-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8360-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a8360-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8360-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8360-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8360-109">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="a8360-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8360-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8360-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8360-111">Not supported.</span></span>                              |
| <span data-ttu-id="a8360-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8360-112">Application</span></span>                            | <span data-ttu-id="a8360-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8360-113">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="a8360-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8360-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="a8360-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8360-115">Request headers</span></span>

| <span data-ttu-id="a8360-116">Имя</span><span class="sxs-lookup"><span data-stu-id="a8360-116">Name</span></span>          | <span data-ttu-id="a8360-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a8360-117">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a8360-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8360-118">Authorization</span></span> | <span data-ttu-id="a8360-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8360-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8360-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8360-121">Request body</span></span>

<span data-ttu-id="a8360-p103">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON. В качестве свойства владельца **PlannerPlan** необходимо указать идентификатор объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="a8360-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="a8360-124">**Примечание:** Пользователь, создающий план, должен быть членом группы, которая будет владельцем плана.</span><span class="sxs-lookup"><span data-stu-id="a8360-124">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="a8360-125">При создании новой группы с помощью кнопки [Создать группу](../api/group_post_groups.md) пользователь не добавляется в группу в качестве члена.</span><span class="sxs-lookup"><span data-stu-id="a8360-125">When you create a new group by using [Create group](../api/group_post_groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="a8360-126">После создания группы добавьте себя в качестве члена с помощью [членов группы с правом записи](../api/group_post_members.md).</span><span class="sxs-lookup"><span data-stu-id="a8360-126">After the group is created, add yourself as a member by using [group post members](../api/group_post_members.md).</span></span>


## <a name="response"></a><span data-ttu-id="a8360-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8360-127">Response</span></span>

<span data-ttu-id="a8360-128">В случае успеха этот метод возвращает код ответа `201 Created` и объект [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8360-128">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="a8360-p105">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a8360-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a8360-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a8360-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8360-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8360-133">Request</span></span>

<span data-ttu-id="a8360-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8360-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="a8360-135">Включите в текст запроса описание объекта [plannerPlan](../resources/plannerplan.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8360-135">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="a8360-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8360-136">Response</span></span>

<span data-ttu-id="a8360-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8360-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
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