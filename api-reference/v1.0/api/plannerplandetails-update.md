---
title: Обновление объекта plannerplandetails
description: Обновление свойств объекта **plannerplandetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 9e706b9e0d95c4084d0b234e81df03905e7aca5e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473852"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="7e3a2-103">Обновление объекта plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="7e3a2-103">Update plannerplandetails</span></span>

<span data-ttu-id="7e3a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e3a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e3a2-105">Обновление свойств объекта **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-105">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e3a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e3a2-106">Permissions</span></span>
<span data-ttu-id="7e3a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e3a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e3a2-109">Permission type</span></span>      | <span data-ttu-id="7e3a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e3a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e3a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e3a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e3a2-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e3a2-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e3a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e3a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e3a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-114">Not supported.</span></span>    |
|<span data-ttu-id="7e3a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e3a2-115">Application</span></span> | <span data-ttu-id="7e3a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e3a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e3a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="7e3a2-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e3a2-118">Optional request headers</span></span>
| <span data-ttu-id="7e3a2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e3a2-119">Name</span></span>       | <span data-ttu-id="7e3a2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7e3a2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e3a2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e3a2-121">Authorization</span></span>  | <span data-ttu-id="7e3a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e3a2-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="7e3a2-124">If-Match</span></span>  | <span data-ttu-id="7e3a2-p103">Последнее известное значение ETag обновляемого объекта plannerPlanDetails. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e3a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e3a2-127">Request body</span></span>
<span data-ttu-id="7e3a2-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e3a2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e3a2-131">Property</span></span>     | <span data-ttu-id="7e3a2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7e3a2-132">Type</span></span>   |<span data-ttu-id="7e3a2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7e3a2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e3a2-134">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7e3a2-134">categoryDescriptions</span></span>|[<span data-ttu-id="7e3a2-135">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7e3a2-135">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="7e3a2-136">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-136">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="7e3a2-137">sharedWith</span><span class="sxs-lookup"><span data-stu-id="7e3a2-137">sharedWith</span></span>|[<span data-ttu-id="7e3a2-138">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="7e3a2-138">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="7e3a2-139">Набор пользовательских ids, с помощью которые мы делим этот план.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-139">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="7e3a2-140">Если вы используете группы Microsoft 365, используйте API групп для управления членством в группе, чтобы поделиться планом [группы.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="7e3a2-140">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan.</span></span> <span data-ttu-id="7e3a2-141">Вы также можете добавить в эту коллекцию существующих членов группы, хотя для них не требуется доступ к плану, который принадлежит группе.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-141">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="7e3a2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e3a2-142">Response</span></span>

<span data-ttu-id="7e3a2-143">В случае успешной работы этот метод возвращает `204 No Content` отклик и пустой контент.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-143">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="7e3a2-144">Если запрос указывает заголовку с предпочтением, этот метод возвращает код ответа и обновленный `Prefer` `return=representation` объект `200 OK` [plannerPlanDetails](../resources/plannerplandetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-144">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="7e3a2-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7e3a2-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7e3a2-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e3a2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e3a2-149">Request</span></span>
<span data-ttu-id="7e3a2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e3a2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e3a2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
Content-type: application/json
Content-length: 212
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7e3a2-152">C#</span><span class="sxs-lookup"><span data-stu-id="7e3a2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e3a2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e3a2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e3a2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e3a2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e3a2-155">Java</span><span class="sxs-lookup"><span data-stu-id="7e3a2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7e3a2-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e3a2-156">Response</span></span>
<span data-ttu-id="7e3a2-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e3a2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

