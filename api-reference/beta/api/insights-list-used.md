---
title: Список, используемый
description: Вычисляемые представление, которое возвращает список файлов, используемых с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: e73536d5933d6293539eb00ba8cdc2e85ce5fa93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526104"
---
# <a name="list-used"></a><span data-ttu-id="cadad-103">Список, используемый</span><span class="sxs-lookup"><span data-stu-id="cadad-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cadad-104">Вычисляемые представление, которое возвращает список файлов, используемых с пользователем.</span><span class="sxs-lookup"><span data-stu-id="cadad-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cadad-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cadad-105">Permissions</span></span>
<span data-ttu-id="cadad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cadad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cadad-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cadad-108">Permission type</span></span>      | <span data-ttu-id="cadad-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cadad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cadad-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cadad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cadad-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cadad-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cadad-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cadad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cadad-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cadad-113">Not supported.</span></span>    |
|<span data-ttu-id="cadad-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cadad-114">Application</span></span> | <span data-ttu-id="cadad-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cadad-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cadad-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cadad-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="cadad-117">Разрешения на запрос возвращает результаты использовавшихся документов других пользователей Упорядочить по «lastModifiedDateTime» и «lastAccessedDateTime» имеет значение «lastModifiedDateTime».</span><span class="sxs-lookup"><span data-stu-id="cadad-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cadad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cadad-118">Optional query parameters</span></span>
<span data-ttu-id="cadad-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cadad-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cadad-120">Можно использовать `$filter` параметр к элементам фильтр, используемый запроса.</span><span class="sxs-lookup"><span data-stu-id="cadad-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="cadad-121">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="cadad-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="cadad-122">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="cadad-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="cadad-123">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="cadad-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="cadad-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cadad-124">Request headers</span></span>
| <span data-ttu-id="cadad-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cadad-125">Header</span></span>       |  <span data-ttu-id="cadad-126">Значение</span><span class="sxs-lookup"><span data-stu-id="cadad-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="cadad-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cadad-127">Authorization</span></span>  | <span data-ttu-id="cadad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cadad-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cadad-130">Accept</span><span class="sxs-lookup"><span data-stu-id="cadad-130">Accept</span></span>  | <span data-ttu-id="cadad-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cadad-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cadad-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cadad-132">Request body</span></span>
<span data-ttu-id="cadad-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cadad-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cadad-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cadad-134">Response</span></span>

<span data-ttu-id="cadad-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и список элементов [используется](../resources/insights-used.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cadad-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cadad-136">Пример</span><span class="sxs-lookup"><span data-stu-id="cadad-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cadad-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cadad-137">Request</span></span>

<span data-ttu-id="cadad-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cadad-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="cadad-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="cadad-139">Response</span></span>

<span data-ttu-id="cadad-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cadad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="cadad-143">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="cadad-143">Expanding resource</span></span>
<span data-ttu-id="cadad-144">Можно развернуть ссылается используемых понимание назначения ресурса.</span><span class="sxs-lookup"><span data-stu-id="cadad-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
