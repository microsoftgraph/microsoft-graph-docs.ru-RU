---
title: Обновление объекта plannertaskdetails
description: Обновление свойств объекта **plannertaskdetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 02c558b1a28ad4348f28c3f7738bf6e2b21ddd3e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473341"
---
# <a name="update-plannertaskdetails"></a><span data-ttu-id="c8d05-103">Обновление объекта plannertaskdetails</span><span class="sxs-lookup"><span data-stu-id="c8d05-103">Update plannertaskdetails</span></span>

<span data-ttu-id="c8d05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8d05-105">Обновление свойств объекта **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="c8d05-105">Update the properties of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8d05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d05-106">Permissions</span></span>
<span data-ttu-id="c8d05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8d05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d05-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d05-109">Permission type</span></span>      | <span data-ttu-id="c8d05-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8d05-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8d05-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8d05-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8d05-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d05-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c8d05-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8d05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8d05-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d05-114">Not supported.</span></span>    |
|<span data-ttu-id="c8d05-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8d05-115">Application</span></span> | <span data-ttu-id="c8d05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d05-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8d05-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8d05-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="c8d05-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8d05-118">Optional request headers</span></span>
| <span data-ttu-id="c8d05-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c8d05-119">Name</span></span>       | <span data-ttu-id="c8d05-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d05-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c8d05-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8d05-121">Authorization</span></span>  | <span data-ttu-id="c8d05-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8d05-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8d05-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="c8d05-124">If-Match</span></span>  | <span data-ttu-id="c8d05-p103">Последнее известное значение ETag обновляемыого объекта **plannerTaskDetails**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8d05-p103">Last known ETag value for the **plannerTaskDetails** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8d05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8d05-127">Request body</span></span>
<span data-ttu-id="c8d05-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c8d05-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8d05-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8d05-131">Property</span></span>     | <span data-ttu-id="c8d05-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c8d05-132">Type</span></span>   |<span data-ttu-id="c8d05-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d05-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8d05-134">checklist</span><span class="sxs-lookup"><span data-stu-id="c8d05-134">checklist</span></span>|[<span data-ttu-id="c8d05-135">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="c8d05-135">plannerChecklistItems</span></span>](../resources/plannerchecklistitems.md)|<span data-ttu-id="c8d05-136">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="c8d05-136">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="c8d05-137">description</span><span class="sxs-lookup"><span data-stu-id="c8d05-137">description</span></span>|<span data-ttu-id="c8d05-138">String</span><span class="sxs-lookup"><span data-stu-id="c8d05-138">String</span></span>|<span data-ttu-id="c8d05-139">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="c8d05-139">Description of the task</span></span>|
|<span data-ttu-id="c8d05-140">previewType</span><span class="sxs-lookup"><span data-stu-id="c8d05-140">previewType</span></span>|<span data-ttu-id="c8d05-141">string</span><span class="sxs-lookup"><span data-stu-id="c8d05-141">string</span></span>|<span data-ttu-id="c8d05-p105">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="c8d05-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="c8d05-145">references</span><span class="sxs-lookup"><span data-stu-id="c8d05-145">references</span></span>|[<span data-ttu-id="c8d05-146">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c8d05-146">plannerExternalReferences</span></span>](../resources/plannerexternalreferences.md)|<span data-ttu-id="c8d05-147">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="c8d05-147">The collection of references on the task.</span></span>|

## <a name="response"></a><span data-ttu-id="c8d05-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8d05-148">Response</span></span>

<span data-ttu-id="c8d05-149">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="c8d05-149">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="c8d05-150">Если запрос указывает заголовку с предпочтением, этот метод возвращает код отклика и обновленный объект `Prefer` `return=representation` `200 OK` [plannerTaskDetails](../resources/plannertaskdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8d05-150">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="c8d05-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c8d05-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c8d05-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c8d05-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8d05-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8d05-155">Request</span></span>
<span data-ttu-id="c8d05-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8d05-156">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8d05-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8d05-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
Content-type: application/json
Content-length: 857
Prefer: return=representation
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
      "isChecked": true
    },
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff":{
      "@odata.type": "microsoft.graph.plannerChecklistItem",
      "isChecked": true,
    },
    "a93c93c5-10a6-4167-9551-8bafa09967a7": null
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="c8d05-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8d05-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c8d05-159">C#</span><span class="sxs-lookup"><span data-stu-id="c8d05-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c8d05-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d05-160">Response</span></span>
<span data-ttu-id="c8d05-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8d05-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannertaskdetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


