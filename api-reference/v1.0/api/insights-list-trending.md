---
title: Список "Популярные"
description: Расчетные данные, возвращающие список элементов, популярных в окружении пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 604a05ab01312707b52274c6276ce044349f0d43
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473194"
---
# <a name="list-trending"></a><span data-ttu-id="3effa-103">Список "Популярные"</span><span class="sxs-lookup"><span data-stu-id="3effa-103">List trending</span></span>

<span data-ttu-id="3effa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3effa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3effa-105">Вычисляемая информация, которая включает список документов, включающих тенденции вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="3effa-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3effa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3effa-106">Permissions</span></span>
<span data-ttu-id="3effa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3effa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3effa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3effa-109">Permission type</span></span>      | <span data-ttu-id="3effa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3effa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3effa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3effa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3effa-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3effa-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3effa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3effa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3effa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3effa-114">Not supported.</span></span>    |
|<span data-ttu-id="3effa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3effa-115">Application</span></span> | <span data-ttu-id="3effa-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3effa-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3effa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3effa-117">HTTP request</span></span>
<span data-ttu-id="3effa-118">Получите список документов, которые будут ходить по пользователю или указанному пользователю:</span><span class="sxs-lookup"><span data-stu-id="3effa-118">Get a list of documents trending around the signed-in user or specified user:</span></span>

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="3effa-119">Расширение ресурса, на который ссылается **трендовая** информация:</span><span class="sxs-lookup"><span data-stu-id="3effa-119">Expand the resource referenced by a **trending** insight:</span></span>

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3effa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3effa-120">Optional query parameters</span></span>
<span data-ttu-id="3effa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3effa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="3effa-122">Параметр запроса можно использовать для `$filter` фильтрации элементов тренда.</span><span class="sxs-lookup"><span data-stu-id="3effa-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="3effa-123">Например, в зависимости от **типа:**</span><span class="sxs-lookup"><span data-stu-id="3effa-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="3effa-124">Или на основе **containerType:**</span><span class="sxs-lookup"><span data-stu-id="3effa-124">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="3effa-125">В [resourceVisualization](../resources/insights-resourcevisualization.md)см. доступные типы и типы контейнеров, которые можно фильтровать.</span><span class="sxs-lookup"><span data-stu-id="3effa-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="3effa-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3effa-126">Request headers</span></span>
| <span data-ttu-id="3effa-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3effa-127">Header</span></span>       |  <span data-ttu-id="3effa-128">Значение</span><span class="sxs-lookup"><span data-stu-id="3effa-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="3effa-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3effa-129">Authorization</span></span>  | <span data-ttu-id="3effa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3effa-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3effa-132">Accept</span><span class="sxs-lookup"><span data-stu-id="3effa-132">Accept</span></span>  | <span data-ttu-id="3effa-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3effa-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3effa-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3effa-134">Request body</span></span>
<span data-ttu-id="3effa-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3effa-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3effa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3effa-136">Response</span></span>

<span data-ttu-id="3effa-137">В случае успешной работы этот метод возвращает код ответа и список элементов `200 OK` [тренда](../resources/insights-trending.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3effa-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="3effa-138">Каждый элемент содержит свойства визуализации для отображения элемента в вашем опыте.</span><span class="sxs-lookup"><span data-stu-id="3effa-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="3effa-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3effa-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3effa-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3effa-140">Request</span></span>
<span data-ttu-id="3effa-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3effa-141">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="3effa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3effa-142">Response</span></span>
<span data-ttu-id="3effa-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3effa-143">Here is an example of the response.</span></span> <span data-ttu-id="3effa-144">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3effa-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3effa-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3effa-145">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="3effa-146">В нижней части страницы см. пример не усеченного ответа.</span><span class="sxs-lookup"><span data-stu-id="3effa-146">See an example un-truncated response at the bottom of the page.</span></span>
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
