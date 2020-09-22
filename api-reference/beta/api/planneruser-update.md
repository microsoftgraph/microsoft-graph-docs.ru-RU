---
title: Обновление plannerUser
description: Обновление свойств объекта plannerUser. Эту операцию можно использовать для добавления или удаления планов из списка избранных планов пользователя, а также для указания планов, которые пользователь просматривал в последнее время.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 5510de45148e3fe9e66d2696f0b117920231e688
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095662"
---
# <a name="update-planneruser"></a><span data-ttu-id="07c56-104">Обновление plannerUser</span><span class="sxs-lookup"><span data-stu-id="07c56-104">Update plannerUser</span></span>

<span data-ttu-id="07c56-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c56-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c56-106">Обновление свойств объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="07c56-106">Update the properties of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="07c56-107">Эту операцию можно использовать для добавления или удаления планов из списка избранных планов пользователя, а также для указания планов, которые пользователь просматривал в последнее время.</span><span class="sxs-lookup"><span data-stu-id="07c56-107">You can use this operation to add or remove plans from a user's favorite plans list, and to indicate which plans the user has recently viewed.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c56-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07c56-108">Permissions</span></span>
<span data-ttu-id="07c56-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c56-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07c56-111">Permission type</span></span>      | <span data-ttu-id="07c56-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07c56-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07c56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07c56-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07c56-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c56-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07c56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07c56-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c56-116">Not supported.</span></span>    |
|<span data-ttu-id="07c56-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07c56-117">Application</span></span> | <span data-ttu-id="07c56-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c56-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07c56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07c56-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/planner
```
## <a name="optional-request-headers"></a><span data-ttu-id="07c56-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07c56-120">Optional request headers</span></span>
| <span data-ttu-id="07c56-121">Имя</span><span class="sxs-lookup"><span data-stu-id="07c56-121">Name</span></span>       | <span data-ttu-id="07c56-122">Описание</span><span class="sxs-lookup"><span data-stu-id="07c56-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="07c56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07c56-123">Authorization</span></span>  | <span data-ttu-id="07c56-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="07c56-124">Bearer {code}.</span></span> <span data-ttu-id="07c56-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="07c56-125">Required.</span></span>|
| <span data-ttu-id="07c56-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="07c56-126">If-Match</span></span>  | <span data-ttu-id="07c56-127">Последнее известное значение ETag для **plannerUser** , которое требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="07c56-127">Last known ETag value for the **plannerUser** to be updated.</span></span> <span data-ttu-id="07c56-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="07c56-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c56-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07c56-129">Request body</span></span>
<span data-ttu-id="07c56-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="07c56-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07c56-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="07c56-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07c56-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="07c56-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07c56-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c56-133">Property</span></span>     | <span data-ttu-id="07c56-134">Тип</span><span class="sxs-lookup"><span data-stu-id="07c56-134">Type</span></span>   |<span data-ttu-id="07c56-135">Описание</span><span class="sxs-lookup"><span data-stu-id="07c56-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07c56-136">фаворитепланреференцес</span><span class="sxs-lookup"><span data-stu-id="07c56-136">favoritePlanReferences</span></span>|<span data-ttu-id="07c56-137">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="07c56-137">[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)</span></span>|<span data-ttu-id="07c56-138">Изменения коллекции, содержащие ссылки на планы, помеченные пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="07c56-138">Changes to the collection containing the references to the plans that the user has marked as a favorite.</span></span>|
|<span data-ttu-id="07c56-139">рецентпланреференцес</span><span class="sxs-lookup"><span data-stu-id="07c56-139">recentPlanReferences</span></span>|<span data-ttu-id="07c56-140">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="07c56-140">[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)</span></span>|<span data-ttu-id="07c56-141">Изменения коллекции, содержащие ссылки на планы, которые пользователь недавно просматривал.</span><span class="sxs-lookup"><span data-stu-id="07c56-141">Changes to the collection containing the references to the plans that the user has recently viewed.</span></span>|

## <a name="response"></a><span data-ttu-id="07c56-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c56-142">Response</span></span>
<span data-ttu-id="07c56-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [plannerUser](../resources/planneruser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07c56-143">If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.</span></span>

<span data-ttu-id="07c56-p107">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="07c56-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="07c56-147">Пример</span><span class="sxs-lookup"><span data-stu-id="07c56-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07c56-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="07c56-148">Request</span></span>
<span data-ttu-id="07c56-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07c56-149">The following is an example of the request.</span></span> <span data-ttu-id="07c56-150">В этом запросе добавляется план "следующее обсуждение выпуска" с ИДЕНТИФИКАТОРом "jd8S5gOaFk2S8aWCIAJz42QAAxtD" в качестве избранного для пользователя и удаляется Plan с ИДЕНТИФИКАТОРом "7oTB5aMIAE2rVo — 1N L7RmQAGX2q" из списка "Избранные планы".</span><span class="sxs-lookup"><span data-stu-id="07c56-150">This request adds the plan "Next Release Discussion" with ID "jd8S5gOaFk2S8aWCIAJz42QAAxtD" as a favorite for the user, and removes plan with ID "7oTB5aMIAE2rVo-1N-L7RmQAGX2q" from the favorite plans list.</span></span>
<span data-ttu-id="07c56-151">Он также обновляет время последнего просмотра плана "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span><span class="sxs-lookup"><span data-stu-id="07c56-151">It also updates the last view time of the plan "jd8S5gOaFk2S8aWCIAJz42QAAxtD".</span></span>
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
##### <a name="response"></a><span data-ttu-id="07c56-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c56-152">Response</span></span>
<span data-ttu-id="07c56-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07c56-153">The following is an example of the response.</span></span> 

><span data-ttu-id="07c56-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07c56-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->


