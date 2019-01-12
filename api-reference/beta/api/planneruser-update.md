---
title: Обновление plannerUser
description: Обновление свойства объекта plannerUser. Эту операцию можно использовать для добавления или удаления планы из пользовательского списка избранных планы и для указания которого планы пользователь недавно просмотра.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 733743ffee8e29d66f2ebe411d127161e7e8eb2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925891"
---
# <a name="update-planneruser"></a><span data-ttu-id="c58ef-104">Обновление plannerUser</span><span class="sxs-lookup"><span data-stu-id="c58ef-104">Update plannerUser</span></span>

> <span data-ttu-id="c58ef-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c58ef-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c58ef-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c58ef-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c58ef-107">Обновление свойства объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="c58ef-107">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="c58ef-108">Эту операцию можно использовать для добавления или удаления планы из пользовательского списка избранных планы и для указания которого планы пользователь недавно просмотра.</span><span class="sxs-lookup"><span data-stu-id="c58ef-108">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="c58ef-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c58ef-109">Permissions</span></span>
<span data-ttu-id="c58ef-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c58ef-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c58ef-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c58ef-112">Permission type</span></span>      | <span data-ttu-id="c58ef-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c58ef-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c58ef-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c58ef-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c58ef-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c58ef-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c58ef-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c58ef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c58ef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c58ef-117">Not supported.</span></span>    |
|<span data-ttu-id="c58ef-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c58ef-118">Application</span></span> | <span data-ttu-id="c58ef-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c58ef-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c58ef-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c58ef-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="c58ef-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c58ef-121">Optional request headers</span></span>
| <span data-ttu-id="c58ef-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c58ef-122">Name</span></span>       | <span data-ttu-id="c58ef-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c58ef-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c58ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c58ef-124">Authorization</span></span>  | <span data-ttu-id="c58ef-p105">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c58ef-p105">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="c58ef-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="c58ef-127">If-Match</span></span>  | <span data-ttu-id="c58ef-128">Последний неизвестное значение ETag для **plannerUser** , который требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="c58ef-128">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="c58ef-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c58ef-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c58ef-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c58ef-130">Request body</span></span>
<span data-ttu-id="c58ef-131">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c58ef-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c58ef-132">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c58ef-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c58ef-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c58ef-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c58ef-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="c58ef-134">Property</span></span>     | <span data-ttu-id="c58ef-135">Тип</span><span class="sxs-lookup"><span data-stu-id="c58ef-135">Type</span></span>   |<span data-ttu-id="c58ef-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c58ef-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c58ef-137">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="c58ef-137">favoritePlanReferences</span></span>|<span data-ttu-id="c58ef-138">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="c58ef-138">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)</span></span>|<span data-ttu-id="c58ef-139">Изменения в коллекцию, содержащую ссылки на планы, которые пользователь отметил в список избранного.</span><span class="sxs-lookup"><span data-stu-id="c58ef-139">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="c58ef-140">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="c58ef-140">recentPlanReferences</span></span>|<span data-ttu-id="c58ef-141">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="c58ef-141">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)</span></span>|<span data-ttu-id="c58ef-142">Коллекция, содержащая ссылки на планы, которые пользователь недавно просмотреть изменения.</span><span class="sxs-lookup"><span data-stu-id="c58ef-142">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="c58ef-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="c58ef-143">Response</span></span>
<span data-ttu-id="c58ef-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [plannerUser](../resources/planneruser.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c58ef-144">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="c58ef-p108">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c58ef-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="c58ef-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c58ef-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c58ef-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c58ef-149">Request</span></span>
<span data-ttu-id="c58ef-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c58ef-150">The following is an example of the request.</span></span> <span data-ttu-id="c58ef-151">Этот запрос добавляет план «Следующего выпуска обсуждений» с Идентификатором «jd8S5gOaFk2S8aWCIAJz42QAAxtD» в список избранного для пользователя и удаляет план с Идентификатором «7oTB5aMIAE2rVo-1N-L7RmQAGX2q» из списка избранных планов.</span><span class="sxs-lookup"><span data-stu-id="c58ef-151">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="c58ef-152">Он также обновляет время последнего представление плана «jd8S5gOaFk2S8aWCIAJz42QAAxtD».</span><span class="sxs-lookup"><span data-stu-id="c58ef-152">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_planneruser"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 504
If-Match: W/"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc="

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": " !",
      "planTitle": "Next Release Discussion"
    },
    "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": null
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    }
  }
}
```
##### <a name="response"></a><span data-ttu-id="c58ef-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="c58ef-153">Response</span></span>
<span data-ttu-id="c58ef-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c58ef-154">The following is an example of the response.</span></span> 

><span data-ttu-id="c58ef-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c58ef-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
