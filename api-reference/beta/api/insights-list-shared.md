---
title: Список "Общие"
description: Расчетные данные, возвращающие список файлов, которыми вы поделились с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 010c2809d4679c2cfdc8090f7c3291ddc8981bfd
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39843831"
---
# <a name="list-shared"></a><span data-ttu-id="d9f78-103">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="d9f78-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f78-104">Вычисляемое представление, включающее список документов, к которым пользователь предоставил доступ.</span><span class="sxs-lookup"><span data-stu-id="d9f78-104">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f78-105">Permissions</span></span>
<span data-ttu-id="d9f78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f78-108">Permission type</span></span>      | <span data-ttu-id="d9f78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9f78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9f78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9f78-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f78-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9f78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9f78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f78-113">Not supported.</span></span>    |
|<span data-ttu-id="d9f78-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9f78-114">Application</span></span> | <span data-ttu-id="d9f78-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f78-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f78-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9f78-116">HTTP request</span></span>
<span data-ttu-id="d9f78-117">Получение списка документов, доступ к которым предоставлен вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="d9f78-117">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="d9f78-118">**Note**: только пользователь может выполнять запросы, используя идентификатор пользователя или имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="d9f78-118">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="d9f78-119">Разверните ресурс, на который ссылается **совместное** представление:</span><span class="sxs-lookup"><span data-stu-id="d9f78-119">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9f78-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d9f78-120">Optional query parameters</span></span>
<span data-ttu-id="d9f78-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d9f78-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d9f78-122">С помощью параметра `$filter` запроса можно фильтровать общие элементы.</span><span class="sxs-lookup"><span data-stu-id="d9f78-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="d9f78-123">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="d9f78-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d9f78-124">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="d9f78-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="d9f78-125">Вы также можете получить файлы, к которым предоставлен доступ конкретному пользователю.</span><span class="sxs-lookup"><span data-stu-id="d9f78-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="d9f78-126">Например, указав `lastshared/sharedby/address` свойство:</span><span class="sxs-lookup"><span data-stu-id="d9f78-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="d9f78-127">Просмотр сложного типа [шарингдетаил](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="d9f78-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d9f78-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9f78-128">Request headers</span></span>
| <span data-ttu-id="d9f78-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9f78-129">Header</span></span>       |  <span data-ttu-id="d9f78-130">Значение</span><span class="sxs-lookup"><span data-stu-id="d9f78-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d9f78-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9f78-131">Authorization</span></span>  | <span data-ttu-id="d9f78-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9f78-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d9f78-134">Accept</span><span class="sxs-lookup"><span data-stu-id="d9f78-134">Accept</span></span>  | <span data-ttu-id="d9f78-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d9f78-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9f78-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9f78-136">Request body</span></span>
<span data-ttu-id="d9f78-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9f78-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9f78-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9f78-138">Response</span></span>

<span data-ttu-id="d9f78-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [общих](../resources/insights-shared.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d9f78-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9f78-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d9f78-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9f78-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9f78-141">Request</span></span>

<span data-ttu-id="d9f78-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9f78-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="d9f78-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f78-143">Response</span></span>

<span data-ttu-id="d9f78-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9f78-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

