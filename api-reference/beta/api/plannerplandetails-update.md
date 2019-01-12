---
title: Обновление объекта plannerplandetails
description: Обновление свойств объекта **plannerplandetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd42196238fb103021debf8a4fee2f658053a255
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950139"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="79da7-103">Обновление объекта plannerplandetails</span><span class="sxs-lookup"><span data-stu-id="79da7-103">Update plannerplandetails</span></span>

> <span data-ttu-id="79da7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79da7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79da7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79da7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79da7-106">Обновление свойств объекта **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="79da7-106">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79da7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79da7-107">Permissions</span></span>
<span data-ttu-id="79da7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79da7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79da7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79da7-110">Permission type</span></span>      | <span data-ttu-id="79da7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79da7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79da7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79da7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79da7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79da7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="79da7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79da7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79da7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79da7-115">Not supported.</span></span>    |
|<span data-ttu-id="79da7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79da7-116">Application</span></span> | <span data-ttu-id="79da7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79da7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79da7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79da7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="79da7-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79da7-119">Optional request headers</span></span>
| <span data-ttu-id="79da7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="79da7-120">Name</span></span>       | <span data-ttu-id="79da7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="79da7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79da7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79da7-122">Authorization</span></span>  | <span data-ttu-id="79da7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79da7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79da7-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="79da7-125">If-Match</span></span>  | <span data-ttu-id="79da7-p104">Последнее известное значение ETag обновляемого объекта plannerPlanDetails. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79da7-p104">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79da7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79da7-128">Request body</span></span>
<span data-ttu-id="79da7-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="79da7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79da7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="79da7-132">Property</span></span>     | <span data-ttu-id="79da7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="79da7-133">Type</span></span>   |<span data-ttu-id="79da7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="79da7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79da7-135">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="79da7-135">categoryDescriptions</span></span>|[<span data-ttu-id="79da7-136">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="79da7-136">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="79da7-137">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="79da7-137">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="79da7-138">sharedWith</span><span class="sxs-lookup"><span data-stu-id="79da7-138">sharedWith</span></span>|[<span data-ttu-id="79da7-139">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="79da7-139">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="79da7-p106">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, используйте API Групп для предоставления доступа к плану [группы](../resources/group.md). Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="79da7-p106">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="79da7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="79da7-143">Response</span></span>

<span data-ttu-id="79da7-144">В случае успеха этот метод возвращает код ответа `200 OK` и обновленный объект [plannerPlanDetails](../resources/plannerplandetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79da7-144">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="79da7-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="79da7-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="79da7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="79da7-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79da7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="79da7-149">Request</span></span>
<span data-ttu-id="79da7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79da7-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
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
##### <a name="response"></a><span data-ttu-id="79da7-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="79da7-151">Response</span></span>
<span data-ttu-id="79da7-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79da7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
