---
title: Список "Популярные"
description: Вычисляемое представление, которое возвращает список элементов, которые обходить пользователь.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49f777e77663a4c055e186860f791459db57ca9c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323701"
---
# <a name="list-trending"></a><span data-ttu-id="9d240-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="9d240-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d240-104">Вычисляемое представление, которое возвращает список элементов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="9d240-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d240-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d240-105">Permissions</span></span>
<span data-ttu-id="9d240-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d240-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d240-108">Permission type</span></span>      | <span data-ttu-id="9d240-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d240-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d240-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d240-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d240-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d240-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d240-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d240-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d240-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d240-113">Not supported.</span></span>    |
|<span data-ttu-id="9d240-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d240-114">Application</span></span> | <span data-ttu-id="9d240-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d240-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d240-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d240-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d240-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d240-117">Optional query parameters</span></span>
<span data-ttu-id="9d240-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d240-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9d240-119">С помощью параметра `$filter` запроса можно фильтровать элементы тенденции.</span><span class="sxs-lookup"><span data-stu-id="9d240-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="9d240-120">Например, на основе типа:</span><span class="sxs-lookup"><span data-stu-id="9d240-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="9d240-121">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="9d240-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="9d240-122">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="9d240-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="9d240-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d240-123">Request headers</span></span>
| <span data-ttu-id="9d240-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d240-124">Header</span></span>       |  <span data-ttu-id="9d240-125">Значение</span><span class="sxs-lookup"><span data-stu-id="9d240-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="9d240-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d240-126">Authorization</span></span>  | <span data-ttu-id="9d240-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d240-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9d240-129">Accept</span><span class="sxs-lookup"><span data-stu-id="9d240-129">Accept</span></span>  | <span data-ttu-id="9d240-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9d240-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d240-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d240-131">Request body</span></span>
<span data-ttu-id="9d240-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d240-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d240-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d240-133">Response</span></span>

<span data-ttu-id="9d240-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список элементов [тенденции](../resources/insights-trending.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d240-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="9d240-135">Каждый элемент содержит свойства зрительного образа для отображения элемента в интерфейсе пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d240-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="9d240-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9d240-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d240-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d240-137">Request</span></span>
<span data-ttu-id="9d240-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d240-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="9d240-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d240-139">Response</span></span>
<span data-ttu-id="9d240-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d240-140">Here is an example of the response.</span></span> <span data-ttu-id="9d240-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9d240-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d240-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d240-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="9d240-143">Пример неусеченного ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="9d240-143">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="9d240-144">Расширение ресурса</span><span class="sxs-lookup"><span data-stu-id="9d240-144">Expanding resource</span></span>
<span data-ttu-id="9d240-145">Ресурс, на который ссылается аналитика оценки тенденций, можно расширить.</span><span class="sxs-lookup"><span data-stu-id="9d240-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
