---
title: Список общих
description: Вычисляемые представление, которое возвращает список файлов, совместно с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2eef2a9b306984a8ad05bcf8fefca2458d609ab1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517353"
---
# <a name="list-shared"></a><span data-ttu-id="06fe4-103">Список общих</span><span class="sxs-lookup"><span data-stu-id="06fe4-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06fe4-104">Вычисляемые представление, которое возвращает список файлов, совместно с пользователем.</span><span class="sxs-lookup"><span data-stu-id="06fe4-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="06fe4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06fe4-105">Permissions</span></span>
<span data-ttu-id="06fe4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fe4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06fe4-108">Permission type</span></span>      | <span data-ttu-id="06fe4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06fe4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06fe4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06fe4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06fe4-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fe4-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="06fe4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06fe4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06fe4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06fe4-113">Not supported.</span></span>    |
|<span data-ttu-id="06fe4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06fe4-114">Application</span></span> | <span data-ttu-id="06fe4-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fe4-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06fe4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06fe4-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="06fe4-117">Запросите с «идентификатор пользователя» или «userPrincipalName» доступно только для пользователя, а не по кому-либо:</span><span class="sxs-lookup"><span data-stu-id="06fe4-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06fe4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06fe4-118">Optional query parameters</span></span>
<span data-ttu-id="06fe4-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06fe4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="06fe4-120">Можно использовать `$filter` параметр для фильтрации общих элементов запроса.</span><span class="sxs-lookup"><span data-stu-id="06fe4-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="06fe4-121">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="06fe4-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="06fe4-122">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="06fe4-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="06fe4-123">Вы также можете получить файлы, общие для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="06fe4-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="06fe4-124">Например, путем указания `lastshared/sharedby/address` свойства:</span><span class="sxs-lookup"><span data-stu-id="06fe4-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="06fe4-125">Сложный тип [sharingDetail](../resources/insights-sharingdetail.md) см.</span><span class="sxs-lookup"><span data-stu-id="06fe4-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="06fe4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06fe4-126">Request headers</span></span>
| <span data-ttu-id="06fe4-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06fe4-127">Header</span></span>       |  <span data-ttu-id="06fe4-128">Значение</span><span class="sxs-lookup"><span data-stu-id="06fe4-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="06fe4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06fe4-129">Authorization</span></span>  | <span data-ttu-id="06fe4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fe4-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="06fe4-132">Accept</span><span class="sxs-lookup"><span data-stu-id="06fe4-132">Accept</span></span>  | <span data-ttu-id="06fe4-133">application/json</span><span class="sxs-lookup"><span data-stu-id="06fe4-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06fe4-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06fe4-134">Request body</span></span>
<span data-ttu-id="06fe4-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06fe4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06fe4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="06fe4-136">Response</span></span>

<span data-ttu-id="06fe4-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и список [общих](../resources/insights-shared.md) элементов в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06fe4-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06fe4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="06fe4-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06fe4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="06fe4-139">Request</span></span>

<span data-ttu-id="06fe4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06fe4-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="06fe4-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="06fe4-141">Response</span></span>

<span data-ttu-id="06fe4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="06fe4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="06fe4-145">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="06fe4-145">Expanding resource</span></span>
<span data-ttu-id="06fe4-146">Можно развернуть ссылается общих сведений об ресурса.</span><span class="sxs-lookup"><span data-stu-id="06fe4-146">The resource referenced by a shared insight can be expanded.</span></span>
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
