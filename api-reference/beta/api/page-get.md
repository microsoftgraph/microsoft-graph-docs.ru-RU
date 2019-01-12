---
title: Получение страницы
description: Получение свойств и связей объекта page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4d583ec28b96b9ec537aaf067371f4ae68fa3375
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979308"
---
# <a name="get-page"></a><span data-ttu-id="15071-103">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="15071-103">Get page</span></span>

> <span data-ttu-id="15071-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15071-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15071-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15071-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15071-106">Получение свойств и связей объекта [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="15071-106">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="15071-107">**Получение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="15071-107">**Getting page information**</span></span>

<span data-ttu-id="15071-108">Доступ к метаданным страницы по ее идентификатору:</span><span class="sxs-lookup"><span data-stu-id="15071-108">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="15071-109">**Получение содержимого страницы**</span><span class="sxs-lookup"><span data-stu-id="15071-109">**Getting page content**</span></span>

<span data-ttu-id="15071-110">Чтобы получить содержимое HTML страницы, вы можете использовать конечную точку `content` страницы:</span><span class="sxs-lookup"><span data-stu-id="15071-110">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="15071-111">Параметр запроса `includeIDs=true` используется для [обновления страниц](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="15071-111">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15071-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15071-112">Permissions</span></span>
<span data-ttu-id="15071-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15071-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15071-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15071-115">Permission type</span></span>      | <span data-ttu-id="15071-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15071-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15071-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15071-117">Delegated (work or school account)</span></span> | <span data-ttu-id="15071-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15071-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="15071-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15071-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15071-120">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15071-120">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="15071-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15071-121">Application</span></span> | <span data-ttu-id="15071-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15071-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15071-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15071-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15071-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15071-124">Optional query parameters</span></span>
<span data-ttu-id="15071-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15071-125">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="15071-p103">Отклик, возвращаемый по умолчанию, разворачивает `parentSection` и выбирает свойства `id`, `name` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="15071-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15071-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15071-128">Request headers</span></span>
| <span data-ttu-id="15071-129">Имя</span><span class="sxs-lookup"><span data-stu-id="15071-129">Name</span></span>       | <span data-ttu-id="15071-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15071-130">Type</span></span> | <span data-ttu-id="15071-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15071-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15071-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="15071-132">Authorization</span></span>  | <span data-ttu-id="15071-133">строка</span><span class="sxs-lookup"><span data-stu-id="15071-133">string</span></span>  | <span data-ttu-id="15071-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15071-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15071-136">Accept</span><span class="sxs-lookup"><span data-stu-id="15071-136">Accept</span></span> | <span data-ttu-id="15071-137">строка</span><span class="sxs-lookup"><span data-stu-id="15071-137">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="15071-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15071-138">Request body</span></span>
<span data-ttu-id="15071-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15071-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15071-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="15071-140">Response</span></span>

<span data-ttu-id="15071-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [page](../resources/page.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15071-141">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15071-142">Пример</span><span class="sxs-lookup"><span data-stu-id="15071-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15071-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="15071-143">Request</span></span>
<span data-ttu-id="15071-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15071-144">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="15071-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="15071-145">Response</span></span>
<span data-ttu-id="15071-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15071-146">Here is an example of the response.</span></span> <span data-ttu-id="15071-147">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="15071-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="15071-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15071-148">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
