---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 51db028e825782f3117d57fecdb7b6ffa4d9639f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404975"
---
# <a name="list-trending"></a><span data-ttu-id="01039-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="01039-103">List trending</span></span>

<span data-ttu-id="01039-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01039-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01039-105">Вычисляемое представление, которое включает в себя список документов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="01039-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="01039-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01039-106">Permissions</span></span>
<span data-ttu-id="01039-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01039-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01039-109">Permission type</span></span>      | <span data-ttu-id="01039-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01039-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01039-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01039-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01039-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01039-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="01039-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01039-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01039-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01039-114">Not supported.</span></span>    |
|<span data-ttu-id="01039-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01039-115">Application</span></span> | <span data-ttu-id="01039-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01039-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01039-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01039-117">HTTP request</span></span>
<span data-ttu-id="01039-118">Получение списка документов, обменяющих пользователя, выполнившего вход, или указанного пользователя:</span><span class="sxs-lookup"><span data-stu-id="01039-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="01039-119">Разверните ресурс, на который ссылается анализ **тенденций** :</span><span class="sxs-lookup"><span data-stu-id="01039-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01039-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01039-120">Optional query parameters</span></span>
<span data-ttu-id="01039-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01039-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="01039-122">`$filter`С помощью параметра запроса можно фильтровать элементы тенденции.</span><span class="sxs-lookup"><span data-stu-id="01039-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="01039-123">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="01039-123">For example, based on **type**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="01039-124">Или на основе **контаинертипе**:</span><span class="sxs-lookup"><span data-stu-id="01039-124">Or based on **containerType**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="01039-125">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="01039-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="01039-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01039-126">Request headers</span></span>
| <span data-ttu-id="01039-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01039-127">Header</span></span>       |  <span data-ttu-id="01039-128">Значение</span><span class="sxs-lookup"><span data-stu-id="01039-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="01039-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01039-129">Authorization</span></span>  | <span data-ttu-id="01039-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01039-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="01039-132">Accept</span><span class="sxs-lookup"><span data-stu-id="01039-132">Accept</span></span>  | <span data-ttu-id="01039-133">application/json</span><span class="sxs-lookup"><span data-stu-id="01039-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01039-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01039-134">Request body</span></span>
<span data-ttu-id="01039-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01039-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01039-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="01039-136">Response</span></span>

<span data-ttu-id="01039-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список элементов [тенденции](../resources/insights-trending.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01039-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="01039-138">Каждый элемент содержит свойства зрительного образа для отображения элемента в интерфейсе пользователя.</span><span class="sxs-lookup"><span data-stu-id="01039-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="01039-139">Если сведения об элементе целевого пользователя отключены, этот метод возвращает результат `403 Forbidden` и следующую ошибку:</span><span class="sxs-lookup"><span data-stu-id="01039-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
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
<span data-ttu-id="01039-140">Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="01039-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="01039-141">Пример</span><span class="sxs-lookup"><span data-stu-id="01039-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01039-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="01039-142">Request</span></span>
<span data-ttu-id="01039-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01039-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01039-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="01039-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="01039-145">C#</span><span class="sxs-lookup"><span data-stu-id="01039-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01039-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01039-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01039-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01039-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="01039-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="01039-148">Response</span></span>
<span data-ttu-id="01039-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01039-149">Here is an example of the response.</span></span> <span data-ttu-id="01039-150">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="01039-150">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="01039-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01039-151">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="01039-152">Пример неусеченного ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="01039-152">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```