---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: e97e5f9a72084b7748551d60e795e43e80f353ed
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844430"
---
# <a name="list-trending"></a><span data-ttu-id="b7ff8-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="b7ff8-103">List trending</span></span>

<span data-ttu-id="b7ff8-104">Вычисляемое представление, которое включает в себя список документов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-104">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7ff8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7ff8-105">Permissions</span></span>
<span data-ttu-id="b7ff8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7ff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7ff8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7ff8-108">Permission type</span></span>      | <span data-ttu-id="b7ff8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7ff8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7ff8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7ff8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7ff8-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7ff8-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7ff8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7ff8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7ff8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-113">Not supported.</span></span>    |
|<span data-ttu-id="b7ff8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7ff8-114">Application</span></span> | <span data-ttu-id="b7ff8-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7ff8-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7ff8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7ff8-116">HTTP request</span></span>
<span data-ttu-id="b7ff8-117">Получение списка документов, обменяющих пользователя, выполнившего вход, или указанного пользователя:</span><span class="sxs-lookup"><span data-stu-id="b7ff8-117">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="b7ff8-118">Разверните ресурс, на который ссылается анализ **тенденций** :</span><span class="sxs-lookup"><span data-stu-id="b7ff8-118">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7ff8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7ff8-119">Optional query parameters</span></span>
<span data-ttu-id="b7ff8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b7ff8-121">С помощью параметра `$filter` запроса можно фильтровать элементы тенденции.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="b7ff8-122">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="b7ff8-122">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="b7ff8-123">Или на основе **контаинертипе**:</span><span class="sxs-lookup"><span data-stu-id="b7ff8-123">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="b7ff8-124">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="b7ff8-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="b7ff8-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7ff8-125">Request headers</span></span>
| <span data-ttu-id="b7ff8-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7ff8-126">Header</span></span>       |  <span data-ttu-id="b7ff8-127">Значение</span><span class="sxs-lookup"><span data-stu-id="b7ff8-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="b7ff8-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7ff8-128">Authorization</span></span>  | <span data-ttu-id="b7ff8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b7ff8-131">Accept</span><span class="sxs-lookup"><span data-stu-id="b7ff8-131">Accept</span></span>  | <span data-ttu-id="b7ff8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b7ff8-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7ff8-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7ff8-133">Request body</span></span>
<span data-ttu-id="b7ff8-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7ff8-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7ff8-135">Response</span></span>

<span data-ttu-id="b7ff8-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список элементов [тенденции](../resources/insights-trending.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="b7ff8-137">Каждый элемент содержит свойства зрительного образа для отображения элемента в интерфейсе пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="b7ff8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b7ff8-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b7ff8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ff8-139">Request</span></span>
<span data-ttu-id="b7ff8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="b7ff8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ff8-141">Response</span></span>
<span data-ttu-id="b7ff8-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-142">Here is an example of the response.</span></span> <span data-ttu-id="b7ff8-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b7ff8-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="b7ff8-145">Пример неусеченного ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="b7ff8-145">See an example un-truncated response at the bottom of the page.</span></span>
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


