---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: f0853d4a215fcb554243a724b1d53d74f848a81d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516712"
---
# <a name="list-trending"></a><span data-ttu-id="cdff1-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="cdff1-103">List trending</span></span>

<span data-ttu-id="cdff1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdff1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdff1-105">Вычисляемое представление, которое включает в себя список документов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="cdff1-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdff1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdff1-106">Permissions</span></span>
<span data-ttu-id="cdff1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cdff1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdff1-109">Permission type</span></span>      | <span data-ttu-id="cdff1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdff1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdff1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdff1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdff1-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdff1-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdff1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdff1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdff1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdff1-114">Not supported.</span></span>    |
|<span data-ttu-id="cdff1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdff1-115">Application</span></span> | <span data-ttu-id="cdff1-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdff1-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdff1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdff1-117">HTTP request</span></span>
<span data-ttu-id="cdff1-118">Получение списка документов, обменяющих пользователя, выполнившего вход, или указанного пользователя:</span><span class="sxs-lookup"><span data-stu-id="cdff1-118">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="cdff1-119">Разверните ресурс, на который ссылается анализ **тенденций** :</span><span class="sxs-lookup"><span data-stu-id="cdff1-119">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdff1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdff1-120">Optional query parameters</span></span>
<span data-ttu-id="cdff1-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdff1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cdff1-122">С помощью параметра `$filter` запроса можно фильтровать элементы тенденции.</span><span class="sxs-lookup"><span data-stu-id="cdff1-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="cdff1-123">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="cdff1-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="cdff1-124">Или на основе **контаинертипе**:</span><span class="sxs-lookup"><span data-stu-id="cdff1-124">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="cdff1-125">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="cdff1-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="cdff1-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdff1-126">Request headers</span></span>
| <span data-ttu-id="cdff1-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdff1-127">Header</span></span>       |  <span data-ttu-id="cdff1-128">Значение</span><span class="sxs-lookup"><span data-stu-id="cdff1-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="cdff1-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdff1-129">Authorization</span></span>  | <span data-ttu-id="cdff1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdff1-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cdff1-132">Accept</span><span class="sxs-lookup"><span data-stu-id="cdff1-132">Accept</span></span>  | <span data-ttu-id="cdff1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="cdff1-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdff1-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdff1-134">Request body</span></span>
<span data-ttu-id="cdff1-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdff1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdff1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdff1-136">Response</span></span>

<span data-ttu-id="cdff1-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список элементов [тенденции](../resources/insights-trending.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdff1-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="cdff1-138">Каждый элемент содержит свойства зрительного образа для отображения элемента в интерфейсе пользователя.</span><span class="sxs-lookup"><span data-stu-id="cdff1-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="cdff1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="cdff1-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cdff1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdff1-140">Request</span></span>
<span data-ttu-id="cdff1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdff1-141">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="cdff1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdff1-142">Response</span></span>
<span data-ttu-id="cdff1-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdff1-143">Here is an example of the response.</span></span> <span data-ttu-id="cdff1-144">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cdff1-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdff1-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdff1-145">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="cdff1-146">Пример неусеченного ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="cdff1-146">See an example un-truncated response at the bottom of the page.</span></span>
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


