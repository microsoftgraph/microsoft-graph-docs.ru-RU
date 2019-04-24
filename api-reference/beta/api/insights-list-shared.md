---
title: Список "Общие"
description: Вычисляемое представление, которое возвращает список файлов, к которым предоставлен доступ пользователю.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 009d9f65b5403139235e5f9afa932ebbe54ff9d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32500388"
---
# <a name="list-shared"></a><span data-ttu-id="c7e87-103">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="c7e87-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e87-104">Вычисляемое представление, которое возвращает список файлов, к которым предоставлен доступ пользователю.</span><span class="sxs-lookup"><span data-stu-id="c7e87-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7e87-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e87-105">Permissions</span></span>
<span data-ttu-id="c7e87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e87-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e87-108">Permission type</span></span>      | <span data-ttu-id="c7e87-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7e87-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7e87-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7e87-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7e87-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e87-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7e87-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7e87-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7e87-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e87-113">Not supported.</span></span>    |
|<span data-ttu-id="c7e87-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7e87-114">Application</span></span> | <span data-ttu-id="c7e87-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e87-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7e87-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7e87-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="c7e87-117">Запрос с идентификатором пользователя или userPrincipalName доступен только пользователю, а не другим пользователям:</span><span class="sxs-lookup"><span data-stu-id="c7e87-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/{id | userPrincipalName}/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7e87-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7e87-118">Optional query parameters</span></span>
<span data-ttu-id="c7e87-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7e87-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c7e87-120">С помощью параметра `$filter` запроса можно фильтровать общие элементы.</span><span class="sxs-lookup"><span data-stu-id="c7e87-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="c7e87-121">Например, на основе типа:</span><span class="sxs-lookup"><span data-stu-id="c7e87-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="c7e87-122">Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="c7e87-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="c7e87-123">Вы также можете получить файлы, к которым предоставлен доступ конкретному пользователю.</span><span class="sxs-lookup"><span data-stu-id="c7e87-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="c7e87-124">Например, указав `lastshared/sharedby/address` свойство:</span><span class="sxs-lookup"><span data-stu-id="c7e87-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="c7e87-125">Просмотр сложного типа [шарингдетаил](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="c7e87-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="c7e87-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7e87-126">Request headers</span></span>
| <span data-ttu-id="c7e87-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7e87-127">Header</span></span>       |  <span data-ttu-id="c7e87-128">Значение</span><span class="sxs-lookup"><span data-stu-id="c7e87-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="c7e87-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7e87-129">Authorization</span></span>  | <span data-ttu-id="c7e87-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7e87-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c7e87-132">Accept</span><span class="sxs-lookup"><span data-stu-id="c7e87-132">Accept</span></span>  | <span data-ttu-id="c7e87-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e87-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e87-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7e87-134">Request body</span></span>
<span data-ttu-id="c7e87-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7e87-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e87-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7e87-136">Response</span></span>

<span data-ttu-id="c7e87-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [общих](../resources/insights-shared.md) элементов в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7e87-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7e87-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c7e87-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c7e87-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7e87-139">Request</span></span>

<span data-ttu-id="c7e87-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7e87-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="c7e87-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7e87-141">Response</span></span>

<span data-ttu-id="c7e87-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7e87-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="c7e87-145">Расширение ресурса</span><span class="sxs-lookup"><span data-stu-id="c7e87-145">Expanding resource</span></span>
<span data-ttu-id="c7e87-146">Ресурс, на который ссылается общая аналитика, может быть расширен.</span><span class="sxs-lookup"><span data-stu-id="c7e87-146">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
