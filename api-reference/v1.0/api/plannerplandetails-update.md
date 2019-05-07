---
title: Обновление объекта plannerplandetails
description: Обновление свойств объекта **plannerplandetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0be66a2edccd8f410f4d3ac73d0a35c6b8e9fdb5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608822"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="131c7-103">Обновление объекта plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="131c7-103">Update plannerplandetails</span></span>

<span data-ttu-id="131c7-104">Обновление свойств объекта **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="131c7-104">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="131c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="131c7-105">Permissions</span></span>
<span data-ttu-id="131c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="131c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="131c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="131c7-108">Permission type</span></span>      | <span data-ttu-id="131c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="131c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="131c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="131c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="131c7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="131c7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="131c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="131c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="131c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="131c7-113">Not supported.</span></span>    |
|<span data-ttu-id="131c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="131c7-114">Application</span></span> | <span data-ttu-id="131c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="131c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="131c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="131c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="131c7-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="131c7-117">Optional request headers</span></span>
| <span data-ttu-id="131c7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="131c7-118">Name</span></span>       | <span data-ttu-id="131c7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="131c7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="131c7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="131c7-120">Authorization</span></span>  | <span data-ttu-id="131c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="131c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="131c7-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="131c7-123">If-Match</span></span>  | <span data-ttu-id="131c7-p103">Последнее известное значение ETag обновляемого объекта plannerPlanDetails. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="131c7-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="131c7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="131c7-126">Request body</span></span>
<span data-ttu-id="131c7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="131c7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="131c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="131c7-130">Property</span></span>     | <span data-ttu-id="131c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="131c7-131">Type</span></span>   |<span data-ttu-id="131c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="131c7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="131c7-133">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="131c7-133">categoryDescriptions</span></span>|[<span data-ttu-id="131c7-134">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="131c7-134">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="131c7-135">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="131c7-135">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="131c7-136">sharedWith</span><span class="sxs-lookup"><span data-stu-id="131c7-136">sharedWith</span></span>|[<span data-ttu-id="131c7-137">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="131c7-137">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="131c7-p105">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, используйте API Групп для предоставления доступа к плану [группы](../resources/group.md). Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="131c7-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="131c7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="131c7-141">Response</span></span>

<span data-ttu-id="131c7-142">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerPlanDetails](../resources/plannerplandetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="131c7-142">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="131c7-p106">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="131c7-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="131c7-146">Пример</span><span class="sxs-lookup"><span data-stu-id="131c7-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="131c7-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="131c7-147">Request</span></span>
<span data-ttu-id="131c7-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="131c7-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
Content-type: application/json
Content-length: 212
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
##### <a name="response"></a><span data-ttu-id="131c7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="131c7-149">Response</span></span>
<span data-ttu-id="131c7-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="131c7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="131c7-153">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="131c7-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="131c7-154">Языках</span><span class="sxs-lookup"><span data-stu-id="131c7-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerplandetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="131c7-155">Язык</span><span class="sxs-lookup"><span data-stu-id="131c7-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerplandetails-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplandetails-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplandetails-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
