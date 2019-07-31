---
title: Список "Популярные"
description: Вычисляемое представление, которое возвращает список элементов, которые обходить пользователь.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 2d84e2c4470b17b3073856a73d0b8cb7251ea830
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953061"
---
# <a name="list-trending"></a><span data-ttu-id="39d51-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="39d51-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39d51-104">Вычисляемое представление, которое возвращает список элементов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="39d51-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="39d51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39d51-105">Permissions</span></span>
<span data-ttu-id="39d51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="39d51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39d51-108">Permission type</span></span>      | <span data-ttu-id="39d51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39d51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39d51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39d51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39d51-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d51-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="39d51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39d51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39d51-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d51-113">Not supported.</span></span>    |
|<span data-ttu-id="39d51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39d51-114">Application</span></span> | <span data-ttu-id="39d51-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d51-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39d51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39d51-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39d51-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39d51-117">Optional query parameters</span></span>
<span data-ttu-id="39d51-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39d51-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="39d51-119">С помощью параметра `$filter` запроса можно фильтровать элементы тенденции.</span><span class="sxs-lookup"><span data-stu-id="39d51-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="39d51-120">Например, на основе типа:</span><span class="sxs-lookup"><span data-stu-id="39d51-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="39d51-121">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="39d51-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="39d51-122">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="39d51-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="39d51-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39d51-123">Request headers</span></span>
| <span data-ttu-id="39d51-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39d51-124">Header</span></span>       |  <span data-ttu-id="39d51-125">Значение</span><span class="sxs-lookup"><span data-stu-id="39d51-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="39d51-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39d51-126">Authorization</span></span>  | <span data-ttu-id="39d51-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39d51-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="39d51-129">Accept</span><span class="sxs-lookup"><span data-stu-id="39d51-129">Accept</span></span>  | <span data-ttu-id="39d51-130">application/json</span><span class="sxs-lookup"><span data-stu-id="39d51-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39d51-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39d51-131">Request body</span></span>
<span data-ttu-id="39d51-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39d51-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39d51-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="39d51-133">Response</span></span>

<span data-ttu-id="39d51-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список элементов [тенденции](../resources/insights-trending.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39d51-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="39d51-135">Каждый элемент содержит свойства зрительного образа для отображения элемента в интерфейсе пользователя.</span><span class="sxs-lookup"><span data-stu-id="39d51-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="39d51-136">Пример</span><span class="sxs-lookup"><span data-stu-id="39d51-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="39d51-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="39d51-137">Request</span></span>
<span data-ttu-id="39d51-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39d51-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="39d51-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="39d51-139">Response</span></span>
<span data-ttu-id="39d51-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39d51-140">Here is an example of the response.</span></span> <span data-ttu-id="39d51-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="39d51-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="39d51-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39d51-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="39d51-143">Пример неусеченного ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="39d51-143">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="39d51-144">Расширение ресурса</span><span class="sxs-lookup"><span data-stu-id="39d51-144">Expanding resource</span></span>
<span data-ttu-id="39d51-145">Ресурс, на который ссылается аналитика оценки тенденций, можно расширить.</span><span class="sxs-lookup"><span data-stu-id="39d51-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
