---
title: Обновление объекта plannertaskdetails
description: Обновление свойств объекта **plannertaskdetails**.
localization_priority: Normal
ms.openlocfilehash: b87688c91a3fe33439c15c403ff248b171a3241e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840196"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="86b34-103">Обновление объекта plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="86b34-103">Update plannertaskdetails</span></span>

<span data-ttu-id="86b34-104">Обновление свойств объекта **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="86b34-104">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86b34-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86b34-105">Permissions</span></span>
<span data-ttu-id="86b34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86b34-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86b34-108">Permission type</span></span>      | <span data-ttu-id="86b34-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86b34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86b34-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86b34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86b34-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b34-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86b34-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86b34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86b34-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86b34-113">Not supported.</span></span>    |
|<span data-ttu-id="86b34-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86b34-114">Application</span></span> | <span data-ttu-id="86b34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86b34-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86b34-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86b34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="86b34-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86b34-117">Optional request headers</span></span>
| <span data-ttu-id="86b34-118">Имя</span><span class="sxs-lookup"><span data-stu-id="86b34-118">Name</span></span>       | <span data-ttu-id="86b34-119">Описание</span><span class="sxs-lookup"><span data-stu-id="86b34-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86b34-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86b34-120">Authorization</span></span>  | <span data-ttu-id="86b34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86b34-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86b34-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="86b34-123">If-Match</span></span>  | <span data-ttu-id="86b34-p103">Последнее известное значение ETag обновляемыого объекта **plannerTaskDetails**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86b34-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86b34-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86b34-126">Request body</span></span>
<span data-ttu-id="86b34-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="86b34-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86b34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86b34-130">Property</span></span>     | <span data-ttu-id="86b34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86b34-131">Type</span></span>   |<span data-ttu-id="86b34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86b34-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86b34-133">checklist</span><span class="sxs-lookup"><span data-stu-id="86b34-133">checklist</span></span>|[<span data-ttu-id="86b34-134">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="86b34-134">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="86b34-135">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="86b34-135">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="86b34-136">описание</span><span class="sxs-lookup"><span data-stu-id="86b34-136">description</span></span>|<span data-ttu-id="86b34-137">Строка</span><span class="sxs-lookup"><span data-stu-id="86b34-137">String</span></span>|<span data-ttu-id="86b34-138">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="86b34-138">Description of the task</span></span>|
|<span data-ttu-id="86b34-139">previewType</span><span class="sxs-lookup"><span data-stu-id="86b34-139">previewType</span></span>|<span data-ttu-id="86b34-140">строка</span><span class="sxs-lookup"><span data-stu-id="86b34-140">string</span></span>|<span data-ttu-id="86b34-141">Задается тип предварительного просмотра, который появляется на задачу.</span><span class="sxs-lookup"><span data-stu-id="86b34-141">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="86b34-142">Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="86b34-142">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="86b34-143">Если параметр имеет значение `automatic` отображаемой предварительного просмотра выбирается по приложению, просмотр задачи.</span><span class="sxs-lookup"><span data-stu-id="86b34-143">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="86b34-144">references</span><span class="sxs-lookup"><span data-stu-id="86b34-144">references</span></span>|[<span data-ttu-id="86b34-145">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="86b34-145">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="86b34-146">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="86b34-146">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="86b34-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="86b34-147">Response</span></span>

<span data-ttu-id="86b34-148">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerTaskDetails](../resources/plannertaskdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="86b34-148">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="86b34-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="86b34-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="86b34-152">Пример</span><span class="sxs-lookup"><span data-stu-id="86b34-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86b34-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="86b34-153">Request</span></span>
<span data-ttu-id="86b34-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86b34-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
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
##### <a name="response"></a><span data-ttu-id="86b34-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="86b34-155">Response</span></span>
<span data-ttu-id="86b34-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="86b34-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
