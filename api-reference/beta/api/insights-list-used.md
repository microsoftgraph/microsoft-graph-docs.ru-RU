---
title: Список "Использованные"
description: Вычисляемое представление, которое возвращает список файлов, используемых с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 31115a845c3b5af80aaba700e55e0ede05d922b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953075"
---
# <a name="list-used"></a><span data-ttu-id="5dcf9-103">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="5dcf9-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dcf9-104">Вычисляемое представление, которое возвращает список файлов, используемых с пользователем.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dcf9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5dcf9-105">Permissions</span></span>
<span data-ttu-id="5dcf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dcf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dcf9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dcf9-108">Permission type</span></span>      | <span data-ttu-id="5dcf9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dcf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dcf9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dcf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5dcf9-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dcf9-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5dcf9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dcf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dcf9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-113">Not supported.</span></span>    |
|<span data-ttu-id="5dcf9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dcf9-114">Application</span></span> | <span data-ttu-id="5dcf9-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dcf9-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dcf9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dcf9-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="5dcf9-117">Запрос документов, использовавшихся другими пользователями возвращает результаты, отсортированные по адресу "lastModifiedDateTime", а для "свойство lastaccesseddatetime" задано значение "lastModifiedDateTime".</span><span class="sxs-lookup"><span data-stu-id="5dcf9-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dcf9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5dcf9-118">Optional query parameters</span></span>
<span data-ttu-id="5dcf9-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5dcf9-120">С помощью параметра `$filter` запроса можно отфильтровать используемые элементы.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="5dcf9-121">Например, на основе типа:</span><span class="sxs-lookup"><span data-stu-id="5dcf9-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="5dcf9-122">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="5dcf9-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="5dcf9-123">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="5dcf9-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="5dcf9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dcf9-124">Request headers</span></span>
| <span data-ttu-id="5dcf9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5dcf9-125">Header</span></span>       |  <span data-ttu-id="5dcf9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="5dcf9-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="5dcf9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5dcf9-127">Authorization</span></span>  | <span data-ttu-id="5dcf9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5dcf9-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5dcf9-130">Accept</span></span>  | <span data-ttu-id="5dcf9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5dcf9-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dcf9-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5dcf9-132">Request body</span></span>
<span data-ttu-id="5dcf9-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dcf9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5dcf9-134">Response</span></span>

<span data-ttu-id="5dcf9-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [использованных](../resources/insights-used.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5dcf9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5dcf9-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5dcf9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dcf9-137">Request</span></span>

<span data-ttu-id="5dcf9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="5dcf9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dcf9-139">Response</span></span>

<span data-ttu-id="5dcf9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="5dcf9-143">Расширение ресурса</span><span class="sxs-lookup"><span data-stu-id="5dcf9-143">Expanding resource</span></span>
<span data-ttu-id="5dcf9-144">Ресурс, на который ссылается использованная аналитика, может быть расширен.</span><span class="sxs-lookup"><span data-stu-id="5dcf9-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
