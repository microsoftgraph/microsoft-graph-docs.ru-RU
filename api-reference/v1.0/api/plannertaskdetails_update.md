# <a name="update-plannertaskdetails"></a><span data-ttu-id="bfae6-101">Обновление объекта plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="bfae6-101">Update plannertaskdetails</span></span>

<span data-ttu-id="bfae6-102">Обновление свойств объекта **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="bfae6-102">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfae6-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfae6-103">Permissions</span></span>
<span data-ttu-id="bfae6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bfae6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bfae6-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfae6-106">Permission type</span></span>      | <span data-ttu-id="bfae6-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfae6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfae6-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfae6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bfae6-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfae6-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfae6-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfae6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfae6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfae6-111">Not supported.</span></span>    |
|<span data-ttu-id="bfae6-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfae6-112">Application</span></span> | <span data-ttu-id="bfae6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfae6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfae6-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfae6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="bfae6-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfae6-115">Optional request headers</span></span>
| <span data-ttu-id="bfae6-116">Имя</span><span class="sxs-lookup"><span data-stu-id="bfae6-116">Name</span></span>       | <span data-ttu-id="bfae6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bfae6-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bfae6-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfae6-118">Authorization</span></span>  | <span data-ttu-id="bfae6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfae6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfae6-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="bfae6-121">If-Match</span></span>  | <span data-ttu-id="bfae6-p103">Последнее известное значение ETag обновляемыого объекта **plannerTaskDetails**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfae6-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfae6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfae6-124">Request body</span></span>
<span data-ttu-id="bfae6-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bfae6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bfae6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfae6-128">Property</span></span>     | <span data-ttu-id="bfae6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bfae6-129">Type</span></span>   |<span data-ttu-id="bfae6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bfae6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfae6-131">checklist</span><span class="sxs-lookup"><span data-stu-id="bfae6-131">checklist</span></span>|[<span data-ttu-id="bfae6-132">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="bfae6-132">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="bfae6-133">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="bfae6-133">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="bfae6-134">description</span><span class="sxs-lookup"><span data-stu-id="bfae6-134">description</span></span>|<span data-ttu-id="bfae6-135">Строка</span><span class="sxs-lookup"><span data-stu-id="bfae6-135">String</span></span>|<span data-ttu-id="bfae6-136">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="bfae6-136">Description of the task</span></span>|
|<span data-ttu-id="bfae6-137">previewType</span><span class="sxs-lookup"><span data-stu-id="bfae6-137">previewType</span></span>|<span data-ttu-id="bfae6-138">string</span><span class="sxs-lookup"><span data-stu-id="bfae6-138">string</span></span>|<span data-ttu-id="bfae6-p105">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="bfae6-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="bfae6-142">references</span><span class="sxs-lookup"><span data-stu-id="bfae6-142">references</span></span>|[<span data-ttu-id="bfae6-143">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="bfae6-143">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="bfae6-144">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="bfae6-144">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="bfae6-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfae6-145">Response</span></span>

<span data-ttu-id="bfae6-146">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerTaskDetails](../resources/plannertaskdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bfae6-146">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="bfae6-p106">Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bfae6-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bfae6-150">Пример</span><span class="sxs-lookup"><span data-stu-id="bfae6-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfae6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfae6-151">Request</span></span>
<span data-ttu-id="bfae6-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfae6-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "previewType": "noPreview",
  "references": {
    "http%3A//developer%2Emicrosoft%2Ecom":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "previewPriority": " !",
      "type": "Other"
    },
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer":{
      "@odata.type": "microsoft.graph.plannerExternalReference",
      "previewPriority": "  !!",
    },
    "http%3A//www%2Ebing%2Ecom": null
  },
  "checklist": {
    "95e27074-6c4a-447a-aa24-9d718a0b86fa":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "title": "Update task details",
      "ischecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
##### <a name="response"></a><span data-ttu-id="bfae6-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfae6-153">Response</span></span>
<span data-ttu-id="bfae6-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bfae6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1793

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "8599273",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "http%3A//developer%2Emicrosoft%2Ecom": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Documentation",
      "type": "Other",
      "previewPriority": "90727736",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Try reading task details",
      "orderHint": "a93c93c5^",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    },
    "95e27074-6c4a-447a-aa24-9d718a0b86f": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": true,
      "title": "Update task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->