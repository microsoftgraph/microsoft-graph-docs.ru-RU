---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5a790c23a0e3cee09079beb5b51151610f309dad
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040247"
---
# <a name="list-trending"></a><span data-ttu-id="2664c-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="2664c-103">List trending</span></span>

<span data-ttu-id="2664c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2664c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2664c-105">Вычисляемая информация, которая включает список документов, включающих тенденции вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="2664c-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2664c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2664c-106">Permissions</span></span>
<span data-ttu-id="2664c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2664c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2664c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2664c-109">Permission type</span></span>      | <span data-ttu-id="2664c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2664c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2664c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2664c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2664c-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2664c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2664c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2664c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2664c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2664c-114">Not supported.</span></span>    |
|<span data-ttu-id="2664c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2664c-115">Application</span></span> | <span data-ttu-id="2664c-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2664c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2664c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2664c-117">HTTP request</span></span>
<span data-ttu-id="2664c-118">Получите список документов, которые будут ходить по пользователю или указанному пользователю:</span><span class="sxs-lookup"><span data-stu-id="2664c-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="2664c-119">Расширение ресурса, на который ссылается **трендовая** информация:</span><span class="sxs-lookup"><span data-stu-id="2664c-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2664c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2664c-120">Optional query parameters</span></span>
<span data-ttu-id="2664c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2664c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="2664c-122">Параметр запроса можно использовать для `$filter` фильтрации элементов тренда.</span><span class="sxs-lookup"><span data-stu-id="2664c-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="2664c-123">Например, в зависимости от **типа:**</span><span class="sxs-lookup"><span data-stu-id="2664c-123">For example, based on **type**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="2664c-124">Или на основе **containerType:**</span><span class="sxs-lookup"><span data-stu-id="2664c-124">Or based on **containerType**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="2664c-125">В [resourceVisualization](../resources/insights-resourcevisualization.md)см. доступные типы и типы контейнеров, которые можно фильтровать.</span><span class="sxs-lookup"><span data-stu-id="2664c-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="2664c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2664c-126">Request headers</span></span>
| <span data-ttu-id="2664c-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2664c-127">Header</span></span>       |  <span data-ttu-id="2664c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="2664c-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="2664c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2664c-129">Authorization</span></span>  | <span data-ttu-id="2664c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2664c-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2664c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="2664c-132">Accept</span></span>  | <span data-ttu-id="2664c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2664c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2664c-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2664c-134">Request body</span></span>
<span data-ttu-id="2664c-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2664c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2664c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2664c-136">Response</span></span>

<span data-ttu-id="2664c-137">В случае успешной работы этот метод возвращает код ответа и список элементов `200 OK` [тренда](../resources/insights-trending.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2664c-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="2664c-138">Каждый элемент содержит свойства визуализации для отображения элемента в вашем опыте.</span><span class="sxs-lookup"><span data-stu-id="2664c-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="2664c-139">Если представление элементов целевого пользователя отключено, этот метод возвращается `403 Forbidden` и следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="2664c-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
<!-- { "blockType": "ignored" } -->

```
{
  "error": {
    "code": "ItemInsightsDisabled",
    "message": " The access to the requested resource is denied because item insights are disabled.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```
<span data-ttu-id="2664c-140">Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="2664c-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="2664c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2664c-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2664c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2664c-142">Request</span></span>
<span data-ttu-id="2664c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2664c-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2664c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2664c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="2664c-145">C#</span><span class="sxs-lookup"><span data-stu-id="2664c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2664c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2664c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2664c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2664c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2664c-148">Java</span><span class="sxs-lookup"><span data-stu-id="2664c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-trending-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2664c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2664c-149">Response</span></span>
<span data-ttu-id="2664c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2664c-150">Here is an example of the response.</span></span> <span data-ttu-id="2664c-151">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2664c-151">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2664c-152">В нижней части страницы см. пример не усеченного ответа.</span><span class="sxs-lookup"><span data-stu-id="2664c-152">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AWMiSOpKHlJCpP_ZoVJQXi9ees4wFhDQQqF55Pm5DlaMzvtd2zra4UWSTEvpTldvb6EhQ289G4BAsxnrajQyjW1jIkjqSh5SQqT_2aFSUF4vBQ",
      "weight": "0.1583399742569597",
      "resourceVisualization": {
        "title": "LiveCaptions",
        "type": "Image",
        "mediaType": "application/octet-stream",
        "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN/thumbnails/0/small/thumbnailContent",
        "previewText": "",
        "containerWebUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared Documents/Go to Market Plan",
        "containerDisplayName": "Mark 8 Project Team",
        "containerType": "Site"
      },
      "resourceReference": {
        "webUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared%20Documents/Go%20to%20Market%20Plan/LiveCaptions.gif",
        "id": "drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN",
        "type": "microsoft.graph.driveItem"
      }
    }
  ]
}
```
