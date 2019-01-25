---
title: Список подписок
description: Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 512dcdfb8a94a2a90c47c4005298537d1d83f137
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525110"
---
# <a name="list-trending"></a><span data-ttu-id="1805b-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="1805b-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1805b-104">Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="1805b-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1805b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1805b-105">Permissions</span></span>
<span data-ttu-id="1805b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1805b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1805b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1805b-108">Permission type</span></span>      | <span data-ttu-id="1805b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1805b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1805b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1805b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1805b-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1805b-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1805b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1805b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1805b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1805b-113">Not supported.</span></span>    |
|<span data-ttu-id="1805b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1805b-114">Application</span></span> | <span data-ttu-id="1805b-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1805b-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1805b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1805b-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1805b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1805b-117">Optional query parameters</span></span>
<span data-ttu-id="1805b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1805b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1805b-119">Можно использовать `$filter` параметр для фильтрации элементов тенденции запроса.</span><span class="sxs-lookup"><span data-stu-id="1805b-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="1805b-120">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="1805b-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="1805b-121">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="1805b-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="1805b-122">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="1805b-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="1805b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1805b-123">Request headers</span></span>
| <span data-ttu-id="1805b-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1805b-124">Header</span></span>       |  <span data-ttu-id="1805b-125">Значение</span><span class="sxs-lookup"><span data-stu-id="1805b-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="1805b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1805b-126">Authorization</span></span>  | <span data-ttu-id="1805b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1805b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1805b-129">Accept</span><span class="sxs-lookup"><span data-stu-id="1805b-129">Accept</span></span>  | <span data-ttu-id="1805b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="1805b-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1805b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1805b-131">Request body</span></span>
<span data-ttu-id="1805b-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1805b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1805b-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1805b-133">Response</span></span>

<span data-ttu-id="1805b-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и список элементов [прибора](../resources/insights-trending.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1805b-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="1805b-135">Каждый элемент содержит свойства визуализации для отображения элемента в работу.</span><span class="sxs-lookup"><span data-stu-id="1805b-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="1805b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1805b-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1805b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1805b-137">Request</span></span>
<span data-ttu-id="1805b-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1805b-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="1805b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1805b-139">Response</span></span>
<span data-ttu-id="1805b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1805b-140">Here is an example of the response.</span></span> <span data-ttu-id="1805b-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1805b-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1805b-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1805b-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="1805b-143">В разделе Пример с усеченными ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="1805b-143">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="1805b-144">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="1805b-144">Expanding resource</span></span>
<span data-ttu-id="1805b-145">Можно развернуть ссылается тенденции понимание назначения ресурса.</span><span class="sxs-lookup"><span data-stu-id="1805b-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
