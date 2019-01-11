---
title: Список общих
description: Вычисляемые представление, которое возвращает список файлов, совместно с пользователем.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: eb9d0165d61559d5f31af486b96e1127c9c7c43c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843269"
---
# <a name="list-shared"></a><span data-ttu-id="4d71d-103">Список общих</span><span class="sxs-lookup"><span data-stu-id="4d71d-103">List shared</span></span>

> <span data-ttu-id="4d71d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d71d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d71d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d71d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d71d-106">Вычисляемые представление, которое возвращает список файлов, совместно с пользователем.</span><span class="sxs-lookup"><span data-stu-id="4d71d-106">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d71d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d71d-107">Permissions</span></span>
<span data-ttu-id="4d71d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d71d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d71d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d71d-110">Permission type</span></span>      | <span data-ttu-id="4d71d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d71d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d71d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d71d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d71d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d71d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d71d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d71d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d71d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d71d-115">Not supported.</span></span>    |
|<span data-ttu-id="4d71d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d71d-116">Application</span></span> | <span data-ttu-id="4d71d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d71d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d71d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d71d-118">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="4d71d-119">Запросите с «идентификатор пользователя» или «userPrincipalName» доступно только для пользователя, а не по кому-либо:</span><span class="sxs-lookup"><span data-stu-id="4d71d-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d71d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d71d-120">Optional query parameters</span></span>
<span data-ttu-id="4d71d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d71d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4d71d-122">Можно использовать `$filter` параметр для фильтрации общих элементов запроса.</span><span class="sxs-lookup"><span data-stu-id="4d71d-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="4d71d-123">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="4d71d-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="4d71d-124">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="4d71d-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="4d71d-125">Вы также можете получить файлы, общие для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d71d-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="4d71d-126">Например, путем указания `lastshared/sharedby/address` свойства:</span><span class="sxs-lookup"><span data-stu-id="4d71d-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="4d71d-127">Сложный тип [sharingDetail](../resources/insights-sharingdetail.md) см.</span><span class="sxs-lookup"><span data-stu-id="4d71d-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="4d71d-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d71d-128">Request headers</span></span>
| <span data-ttu-id="4d71d-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d71d-129">Header</span></span>       |  <span data-ttu-id="4d71d-130">Значение</span><span class="sxs-lookup"><span data-stu-id="4d71d-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="4d71d-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d71d-131">Authorization</span></span>  | <span data-ttu-id="4d71d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d71d-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4d71d-134">Accept</span><span class="sxs-lookup"><span data-stu-id="4d71d-134">Accept</span></span>  | <span data-ttu-id="4d71d-135">application/json</span><span class="sxs-lookup"><span data-stu-id="4d71d-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d71d-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4d71d-136">Request body</span></span>
<span data-ttu-id="4d71d-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d71d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d71d-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d71d-138">Response</span></span>

<span data-ttu-id="4d71d-139">Успешно завершена, этот метод возвращает `200 OK` код ответа и список [общих](../resources/insights-shared.md) элементов в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4d71d-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d71d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4d71d-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d71d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d71d-141">Request</span></span>

<span data-ttu-id="4d71d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d71d-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="4d71d-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d71d-143">Response</span></span>

<span data-ttu-id="4d71d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d71d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="4d71d-147">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="4d71d-147">Expanding resource</span></span>
<span data-ttu-id="4d71d-148">Можно развернуть ссылается общих сведений об ресурса.</span><span class="sxs-lookup"><span data-stu-id="4d71d-148">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
