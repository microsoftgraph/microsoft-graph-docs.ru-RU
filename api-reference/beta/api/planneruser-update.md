---
title: Обновление plannerUser
description: Обновление свойств объекта plannerUser. Эту операцию можно использовать для добавления или удаления планов из списка избранных планов пользователя, а также для указания планов, которые пользователь просматривал в последнее время.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95c631d39fb650dea0b87871bdd10d92a3ab31eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538758"
---
# <a name="update-planneruser"></a><span data-ttu-id="4822c-104">Обновление plannerUser</span><span class="sxs-lookup"><span data-stu-id="4822c-104">Update plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4822c-105">Обновление свойств объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="4822c-105">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="4822c-106">Эту операцию можно использовать для добавления или удаления планов из списка избранных планов пользователя, а также для указания планов, которые пользователь просматривал в последнее время.</span><span class="sxs-lookup"><span data-stu-id="4822c-106">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="4822c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4822c-107">Permissions</span></span>
<span data-ttu-id="4822c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4822c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4822c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4822c-110">Permission type</span></span>      | <span data-ttu-id="4822c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4822c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4822c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4822c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4822c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4822c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4822c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4822c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4822c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4822c-115">Not supported.</span></span>    |
|<span data-ttu-id="4822c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4822c-116">Application</span></span> | <span data-ttu-id="4822c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4822c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4822c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4822c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="4822c-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4822c-119">Optional request headers</span></span>
| <span data-ttu-id="4822c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4822c-120">Name</span></span>       | <span data-ttu-id="4822c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4822c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4822c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4822c-122">Authorization</span></span>  | <span data-ttu-id="4822c-123">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="4822c-123">Bearer {code}.</span></span> <span data-ttu-id="4822c-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4822c-124">Required.</span></span>|
| <span data-ttu-id="4822c-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="4822c-125">If-Match</span></span>  | <span data-ttu-id="4822c-126">Последнее известное значение ETag для **plannerUser** , которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="4822c-126">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="4822c-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4822c-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4822c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4822c-128">Request body</span></span>
<span data-ttu-id="4822c-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4822c-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4822c-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4822c-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4822c-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4822c-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4822c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4822c-132">Property</span></span>     | <span data-ttu-id="4822c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4822c-133">Type</span></span>   |<span data-ttu-id="4822c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4822c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4822c-135">Фаворитепланреференцес</span><span class="sxs-lookup"><span data-stu-id="4822c-135">favoritePlanReferences</span></span>|<span data-ttu-id="4822c-136">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="4822c-136">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)</span></span>|<span data-ttu-id="4822c-137">Изменения коллекции, содержащие ссылки на планы, помеченные пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="4822c-137">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="4822c-138">Рецентпланреференцес</span><span class="sxs-lookup"><span data-stu-id="4822c-138">recentPlanReferences</span></span>|<span data-ttu-id="4822c-139">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="4822c-139">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)</span></span>|<span data-ttu-id="4822c-140">Изменения коллекции, содержащие ссылки на планы, которые пользователь недавно просматривал.</span><span class="sxs-lookup"><span data-stu-id="4822c-140">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="4822c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4822c-141">Response</span></span>
<span data-ttu-id="4822c-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerUser](../resources/planneruser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4822c-142">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="4822c-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4822c-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="4822c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4822c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4822c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4822c-147">Request</span></span>
<span data-ttu-id="4822c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4822c-148">The following is an example of the request.</span></span> <span data-ttu-id="4822c-149">В этом запросе добавляется план "следующее обсуждение выпуска" с ИДЕНТИФИКАТОРом "jd8S5gOaFk2S8aWCIAJz42QAAxtD" в качестве избранного для пользователя и удаляется Plan с ИДЕНТИФИКАТОРом "7oTB5aMIAE2rVo — 1N L7RmQAGX2q" из списка "Избранные планы".</span><span class="sxs-lookup"><span data-stu-id="4822c-149">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="4822c-150">Он также обновляет время последнего просмотра плана "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="4822c-150">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="4822c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4822c-151">Response</span></span>
<span data-ttu-id="4822c-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4822c-152">The following is an example of the response.</span></span> 

><span data-ttu-id="4822c-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4822c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
