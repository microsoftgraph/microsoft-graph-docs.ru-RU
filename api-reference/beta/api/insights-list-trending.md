---
title: Список подписок
description: Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.
ms.openlocfilehash: 94433d094c2ab527e33ac04730cdbb72a1b94c1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078663"
---
# <a name="list-trending"></a><span data-ttu-id="2020d-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="2020d-103">List trending</span></span>

> <span data-ttu-id="2020d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2020d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2020d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2020d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2020d-106">Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="2020d-106">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2020d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2020d-107">Permissions</span></span>
<span data-ttu-id="2020d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2020d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2020d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2020d-110">Permission type</span></span>      | <span data-ttu-id="2020d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2020d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2020d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2020d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2020d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2020d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2020d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2020d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2020d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2020d-115">Not supported.</span></span>    |
|<span data-ttu-id="2020d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2020d-116">Application</span></span> | <span data-ttu-id="2020d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2020d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2020d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2020d-118">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2020d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2020d-119">Optional query parameters</span></span>
<span data-ttu-id="2020d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2020d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2020d-121">Можно использовать `$filter` параметр для фильтрации элементов тенденции запроса.</span><span class="sxs-lookup"><span data-stu-id="2020d-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="2020d-122">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="2020d-122">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="2020d-123">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="2020d-123">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="2020d-124">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="2020d-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="2020d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2020d-125">Request headers</span></span>
| <span data-ttu-id="2020d-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2020d-126">Header</span></span>       |  <span data-ttu-id="2020d-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2020d-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="2020d-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2020d-128">Authorization</span></span>  | <span data-ttu-id="2020d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2020d-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2020d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="2020d-131">Accept</span></span>  | <span data-ttu-id="2020d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2020d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2020d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2020d-133">Request body</span></span>
<span data-ttu-id="2020d-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2020d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2020d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2020d-135">Response</span></span>

<span data-ttu-id="2020d-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и список элементов [прибора](../resources/insights-trending.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2020d-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="2020d-137">Каждый элемент содержит свойства визуализации для отображения элемента в работу.</span><span class="sxs-lookup"><span data-stu-id="2020d-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="2020d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2020d-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2020d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2020d-139">Request</span></span>
<span data-ttu-id="2020d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2020d-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="2020d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2020d-141">Response</span></span>
<span data-ttu-id="2020d-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2020d-142">Here is an example of the response.</span></span> <span data-ttu-id="2020d-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2020d-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2020d-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2020d-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="2020d-145">В разделе Пример с усеченными ответа в нижней части страницы.</span><span class="sxs-lookup"><span data-stu-id="2020d-145">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="2020d-146">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="2020d-146">Expanding resource</span></span>
<span data-ttu-id="2020d-147">Можно развернуть ссылается тенденции понимание назначения ресурса.</span><span class="sxs-lookup"><span data-stu-id="2020d-147">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
