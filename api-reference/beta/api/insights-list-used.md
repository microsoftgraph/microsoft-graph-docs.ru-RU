---
title: Список "Использованные"
description: Расчетные данные, возвращающие список файлов, которые вы используете вместе с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 3bd97a9c727a88cd4677de359880c79ed8a85e39
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39843870"
---
# <a name="list-used"></a><span data-ttu-id="cf317-103">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="cf317-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf317-104">Вычисляемое представление, содержащее список документов, измененных пользователем.</span><span class="sxs-lookup"><span data-stu-id="cf317-104">Calculated insight that includes a list of documents the user has modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf317-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf317-105">Permissions</span></span>
<span data-ttu-id="cf317-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf317-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf317-108">Permission type</span></span>      | <span data-ttu-id="cf317-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf317-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf317-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf317-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf317-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf317-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf317-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf317-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf317-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf317-113">Not supported.</span></span>    |
|<span data-ttu-id="cf317-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf317-114">Application</span></span> | <span data-ttu-id="cf317-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf317-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf317-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf317-116">HTTP request</span></span>
<span data-ttu-id="cf317-117">Получение списка документов, измененных пользователем, вошедших в систему:</span><span class="sxs-lookup"><span data-stu-id="cf317-117">Get a list of documents that the signed-in user has modified:</span></span>

```http
GET /me/insights/used
```

<span data-ttu-id="cf317-118">Получение списка документов, измененных указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="cf317-118">Get a list of documents that the specified user has modified.</span></span>

><span data-ttu-id="cf317-119">**Примечание**. Запрос документов, **использованных** другим пользователем, возвращает результаты, отсортированные по **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="cf317-119">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="cf317-120">Затем для **свойство lastaccesseddatetime** устанавливается значение **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="cf317-120">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>
```http
GET /users/{id | userPrincipalName}/insights/used
```

<span data-ttu-id="cf317-121">Разверните ресурс, на который ссылается **использованная** аналитика:</span><span class="sxs-lookup"><span data-stu-id="cf317-121">Expand the resource referenced by a **used** insight:</span></span>

```http
GET /me/insights/used/{id}/resource
GET /users/{id | userPrincipalName}/insights/used/{id}/resource
```


## <a name="optional-query-parameters"></a><span data-ttu-id="cf317-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf317-122">Optional query parameters</span></span>
<span data-ttu-id="cf317-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf317-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cf317-124">С помощью параметра `$filter` запроса можно отфильтровать используемые элементы.</span><span class="sxs-lookup"><span data-stu-id="cf317-124">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="cf317-125">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="cf317-125">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="cf317-126">Или на основе **контаинертипе**:</span><span class="sxs-lookup"><span data-stu-id="cf317-126">Or based on **containerType**:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="cf317-127">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="cf317-127">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="cf317-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf317-128">Request headers</span></span>
| <span data-ttu-id="cf317-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf317-129">Header</span></span>       |  <span data-ttu-id="cf317-130">Значение</span><span class="sxs-lookup"><span data-stu-id="cf317-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="cf317-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf317-131">Authorization</span></span>  | <span data-ttu-id="cf317-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf317-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cf317-134">Accept</span><span class="sxs-lookup"><span data-stu-id="cf317-134">Accept</span></span>  | <span data-ttu-id="cf317-135">application/json</span><span class="sxs-lookup"><span data-stu-id="cf317-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf317-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf317-136">Request body</span></span>
<span data-ttu-id="cf317-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf317-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf317-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf317-138">Response</span></span>

<span data-ttu-id="cf317-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [использованных](../resources/insights-used.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf317-139">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf317-140">Пример</span><span class="sxs-lookup"><span data-stu-id="cf317-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf317-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf317-141">Request</span></span>

<span data-ttu-id="cf317-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf317-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="cf317-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf317-143">Response</span></span>

<span data-ttu-id="cf317-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf317-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

