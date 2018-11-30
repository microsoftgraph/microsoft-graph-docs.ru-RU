---
title: Список, используемый
description: Вычисляемые представление, которое возвращает список файлов, используемых с пользователем.
ms.openlocfilehash: a9e5390e38e4e697f55676304edb4544e4c2ded5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079280"
---
# <a name="list-used"></a><span data-ttu-id="7f961-103">Список, используемый</span><span class="sxs-lookup"><span data-stu-id="7f961-103">List used</span></span>

> <span data-ttu-id="7f961-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f961-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f961-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f961-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f961-106">Вычисляемые представление, которое возвращает список файлов, используемых с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7f961-106">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f961-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f961-107">Permissions</span></span>
<span data-ttu-id="7f961-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f961-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f961-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f961-110">Permission type</span></span>      | <span data-ttu-id="7f961-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f961-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f961-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f961-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f961-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f961-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f961-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f961-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f961-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f961-115">Not supported.</span></span>    |
|<span data-ttu-id="7f961-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f961-116">Application</span></span> | <span data-ttu-id="7f961-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f961-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f961-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f961-118">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="7f961-119">Разрешения на запрос возвращает результаты использовавшихся документов других пользователей Упорядочить по «lastModifiedDateTime» и «lastAccessedDateTime» имеет значение «lastModifiedDateTime».</span><span class="sxs-lookup"><span data-stu-id="7f961-119">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f961-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f961-120">Optional query parameters</span></span>
<span data-ttu-id="7f961-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f961-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7f961-122">Можно использовать `$filter` параметр к элементам фильтр, используемый запроса.</span><span class="sxs-lookup"><span data-stu-id="7f961-122">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="7f961-123">Например на основе типа:</span><span class="sxs-lookup"><span data-stu-id="7f961-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="7f961-124">Или на основе типа контейнера:</span><span class="sxs-lookup"><span data-stu-id="7f961-124">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="7f961-125">В разделе Доступные типы контейнеров и типов можно фильтровать по в [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="7f961-125">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="7f961-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f961-126">Request headers</span></span>
| <span data-ttu-id="7f961-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f961-127">Header</span></span>       |  <span data-ttu-id="7f961-128">Значение</span><span class="sxs-lookup"><span data-stu-id="7f961-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="7f961-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f961-129">Authorization</span></span>  | <span data-ttu-id="7f961-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f961-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="7f961-132">Accept</span><span class="sxs-lookup"><span data-stu-id="7f961-132">Accept</span></span>  | <span data-ttu-id="7f961-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7f961-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f961-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f961-134">Request body</span></span>
<span data-ttu-id="7f961-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f961-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f961-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f961-136">Response</span></span>

<span data-ttu-id="7f961-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и список элементов [используется](../resources/insights-used.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7f961-137">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f961-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7f961-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f961-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f961-139">Request</span></span>

<span data-ttu-id="7f961-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f961-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="7f961-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f961-141">Response</span></span>

<span data-ttu-id="7f961-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7f961-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="7f961-145">Развертывание ресурсов</span><span class="sxs-lookup"><span data-stu-id="7f961-145">Expanding resource</span></span>
<span data-ttu-id="7f961-146">Можно развернуть ссылается используемых понимание назначения ресурса.</span><span class="sxs-lookup"><span data-stu-id="7f961-146">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
