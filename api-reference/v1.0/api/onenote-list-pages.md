---
title: Перечисление страниц
description: Получение списка объектов page.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5a7796bad3afbb7f30b6200f20b667fe53cc0c89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955648"
---
# <a name="list-pages"></a><span data-ttu-id="9a9cc-103">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="9a9cc-103">List pages</span></span>

<span data-ttu-id="9a9cc-104">Получение списка объектов [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="9a9cc-104">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a9cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a9cc-105">Permissions</span></span>
<span data-ttu-id="9a9cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a9cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a9cc-108">Permission type</span></span>      | <span data-ttu-id="9a9cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a9cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a9cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a9cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a9cc-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a9cc-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a9cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a9cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a9cc-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a9cc-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9a9cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a9cc-114">Application</span></span> | <span data-ttu-id="9a9cc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a9cc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a9cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a9cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a9cc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a9cc-117">Optional query parameters</span></span>
<span data-ttu-id="9a9cc-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9a9cc-p102">Запрос страниц по умолчанию возвращает первые 20 страниц, упорядоченные по атрибуту `lastModifiedTime desc`. Если запрос по умолчанию возвращает более 20 страниц, ответ содержит URL-адрес `@odata.nextLink`, который можно использовать для перехода на следующую страницу результатов. Максимальное количество страниц, возвращаемых по запросу `top`, — 100.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="9a9cc-p103">Ответ по умолчанию разворачивает `parentSection` и выбирает свойства `id`, `displayName` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a9cc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a9cc-124">Request headers</span></span>
| <span data-ttu-id="9a9cc-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9a9cc-125">Name</span></span>       | <span data-ttu-id="9a9cc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9a9cc-126">Type</span></span> | <span data-ttu-id="9a9cc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9cc-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9a9cc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a9cc-128">Authorization</span></span>  | <span data-ttu-id="9a9cc-129">строка</span><span class="sxs-lookup"><span data-stu-id="9a9cc-129">string</span></span>  | <span data-ttu-id="9a9cc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a9cc-132">Accept</span><span class="sxs-lookup"><span data-stu-id="9a9cc-132">Accept</span></span> | <span data-ttu-id="9a9cc-133">строка</span><span class="sxs-lookup"><span data-stu-id="9a9cc-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9a9cc-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a9cc-134">Request body</span></span>
<span data-ttu-id="9a9cc-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a9cc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a9cc-136">Response</span></span>

<span data-ttu-id="9a9cc-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-137">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a9cc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9a9cc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a9cc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a9cc-139">Request</span></span>
<span data-ttu-id="9a9cc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-140">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="9a9cc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a9cc-141">Response</span></span>
<span data-ttu-id="9a9cc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-142">Here is an example of the response.</span></span> <span data-ttu-id="9a9cc-143">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-143">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="9a9cc-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a9cc-144">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
    {
      "title": "title-value",
      "createdByAppId": "createdByAppId-value",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
