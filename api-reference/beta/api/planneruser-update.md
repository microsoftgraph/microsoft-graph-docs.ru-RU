---
title: Обновление plannerUser
description: Обновление свойства объекта plannerUser. Эту операцию можно использовать для добавления или удаления планы из пользовательского списка избранных планы и для указания которого планы пользователь недавно просмотра.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508925"
---
# <a name="update-planneruser"></a><span data-ttu-id="dffbf-104">Обновление plannerUser</span><span class="sxs-lookup"><span data-stu-id="dffbf-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dffbf-105">Обновление свойства объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="dffbf-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="dffbf-106">Эту операцию можно использовать для добавления или удаления планы из пользовательского списка избранных планы и для указания которого планы пользователь недавно просмотра.</span><span class="sxs-lookup"><span data-stu-id="dffbf-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="dffbf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dffbf-107">Permissions</span></span>
<span data-ttu-id="dffbf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dffbf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dffbf-110">Permission type</span></span>      | <span data-ttu-id="dffbf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dffbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dffbf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dffbf-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dffbf-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dffbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dffbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffbf-115">Not supported.</span></span>    |
|<span data-ttu-id="dffbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dffbf-116">Application</span></span> | <span data-ttu-id="dffbf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffbf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dffbf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="dffbf-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dffbf-119">Optional request headers</span></span>
| <span data-ttu-id="dffbf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dffbf-120">Name</span></span>       | <span data-ttu-id="dffbf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dffbf-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dffbf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dffbf-122">Authorization</span></span>  | <span data-ttu-id="dffbf-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dffbf-p104">Bearer {code}. Required.</span></span>|
| <span data-ttu-id="dffbf-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="dffbf-125">If-Match</span></span>  | <span data-ttu-id="dffbf-126">Последний неизвестное значение ETag для **plannerUser** , который требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="dffbf-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="dffbf-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dffbf-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dffbf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dffbf-128">Request body</span></span>
<span data-ttu-id="dffbf-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dffbf-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dffbf-130">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dffbf-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dffbf-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dffbf-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dffbf-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dffbf-132">Property</span></span>     | <span data-ttu-id="dffbf-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dffbf-133">Type</span></span>   |<span data-ttu-id="dffbf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dffbf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dffbf-135">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="dffbf-135">favoritePlanReferences</span></span>|<span data-ttu-id="dffbf-136">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="dffbf-136">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)</span></span>|<span data-ttu-id="dffbf-137">Изменения в коллекцию, содержащую ссылки на планы, которые пользователь отметил в список избранного.</span><span class="sxs-lookup"><span data-stu-id="dffbf-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="dffbf-138">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="dffbf-138">recentPlanReferences</span></span>|<span data-ttu-id="dffbf-139">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="dffbf-139">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)</span></span>|<span data-ttu-id="dffbf-140">Коллекция, содержащая ссылки на планы, которые пользователь недавно просмотреть изменения.</span><span class="sxs-lookup"><span data-stu-id="dffbf-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="dffbf-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="dffbf-141">Response</span></span>
<span data-ttu-id="dffbf-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [plannerUser](../resources/planneruser.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dffbf-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="dffbf-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="dffbf-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="dffbf-146">Пример</span><span class="sxs-lookup"><span data-stu-id="dffbf-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dffbf-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="dffbf-147">Request</span></span>
<span data-ttu-id="dffbf-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dffbf-148">The following is an example of the request.</span></span> <span data-ttu-id="dffbf-149">Этот запрос добавляет план «Следующего выпуска обсуждений» с Идентификатором «jd8S5gOaFk2S8aWCIAJz42QAAxtD» в список избранного для пользователя и удаляет план с Идентификатором «7oTB5aMIAE2rVo-1N-L7RmQAGX2q» из списка избранных планов.</span><span class="sxs-lookup"><span data-stu-id="dffbf-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="dffbf-150">Он также обновляет время последнего представление плана «jd8S5gOaFk2S8aWCIAJz42QAAxtD».</span><span class="sxs-lookup"><span data-stu-id="dffbf-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="dffbf-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="dffbf-151">Response</span></span>
<span data-ttu-id="dffbf-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dffbf-152">The following is an example of the response.</span></span> 

><span data-ttu-id="dffbf-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dffbf-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update planneruser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
