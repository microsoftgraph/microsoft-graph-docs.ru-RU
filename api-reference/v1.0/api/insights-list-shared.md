---
title: Список "Общие"
description: Расчетные данные, возвращающие список файлов, которыми вы поделились с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5ee215dff7fafaa25e4601ade1819322d8894e5a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401577"
---
# <a name="list-shared"></a><span data-ttu-id="2b60c-103">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="2b60c-103">List shared</span></span>

<span data-ttu-id="2b60c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b60c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b60c-105">Вычисляемое представление, включающее список документов, к которым пользователь предоставил доступ.</span><span class="sxs-lookup"><span data-stu-id="2b60c-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b60c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b60c-106">Permissions</span></span>
<span data-ttu-id="2b60c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b60c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b60c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b60c-109">Permission type</span></span>      | <span data-ttu-id="2b60c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b60c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b60c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b60c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b60c-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b60c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b60c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b60c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b60c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b60c-114">Not supported.</span></span>    |
|<span data-ttu-id="2b60c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b60c-115">Application</span></span> | <span data-ttu-id="2b60c-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b60c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b60c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b60c-117">HTTP request</span></span>
<span data-ttu-id="2b60c-118">Получение списка документов, доступ к которым предоставлен вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b60c-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="2b60c-119">**Note**: только пользователь может выполнять запросы, используя идентификатор пользователя или имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="2b60c-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="2b60c-120">Разверните ресурс, на который ссылается **совместное** представление:</span><span class="sxs-lookup"><span data-stu-id="2b60c-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b60c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b60c-121">Optional query parameters</span></span>
<span data-ttu-id="2b60c-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b60c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="2b60c-123">`$filter`С помощью параметра запроса можно фильтровать общие элементы.</span><span class="sxs-lookup"><span data-stu-id="2b60c-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="2b60c-124">Например, на основе **типа**:</span><span class="sxs-lookup"><span data-stu-id="2b60c-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="2b60c-125">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="2b60c-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="2b60c-126">Вы также можете получить файлы, к которым предоставлен доступ конкретному пользователю.</span><span class="sxs-lookup"><span data-stu-id="2b60c-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="2b60c-127">Например, указав `lastshared/sharedby/address` свойство:</span><span class="sxs-lookup"><span data-stu-id="2b60c-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="2b60c-128">Просмотр сложного типа [шарингдетаил](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="2b60c-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2b60c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b60c-129">Request headers</span></span>
| <span data-ttu-id="2b60c-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b60c-130">Header</span></span>       |  <span data-ttu-id="2b60c-131">Значение</span><span class="sxs-lookup"><span data-stu-id="2b60c-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="2b60c-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b60c-132">Authorization</span></span>  | <span data-ttu-id="2b60c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b60c-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2b60c-135">Accept</span><span class="sxs-lookup"><span data-stu-id="2b60c-135">Accept</span></span>  | <span data-ttu-id="2b60c-136">application/json</span><span class="sxs-lookup"><span data-stu-id="2b60c-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b60c-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b60c-137">Request body</span></span>
<span data-ttu-id="2b60c-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b60c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b60c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b60c-139">Response</span></span>

<span data-ttu-id="2b60c-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [общих](../resources/insights-shared.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b60c-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b60c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2b60c-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b60c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b60c-142">Request</span></span>

<span data-ttu-id="2b60c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b60c-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="2b60c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b60c-144">Response</span></span>

<span data-ttu-id="2b60c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b60c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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