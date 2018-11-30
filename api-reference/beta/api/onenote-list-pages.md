---
title: Перечисление страниц
description: Получение списка объектов page.
ms.openlocfilehash: 9144d443b7fe73cc2720c85adb4199ae6ab9a589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082864"
---
# <a name="list-pages"></a><span data-ttu-id="241b7-103">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="241b7-103">List pages</span></span>

> <span data-ttu-id="241b7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="241b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="241b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="241b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="241b7-106">Получение списка объектов [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="241b7-106">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="241b7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="241b7-107">Permissions</span></span>
<span data-ttu-id="241b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="241b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="241b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="241b7-110">Permission type</span></span>      | <span data-ttu-id="241b7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="241b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="241b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="241b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="241b7-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="241b7-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="241b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="241b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="241b7-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="241b7-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="241b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="241b7-116">Application</span></span> | <span data-ttu-id="241b7-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="241b7-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="241b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="241b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="241b7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="241b7-119">Optional query parameters</span></span>
<span data-ttu-id="241b7-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="241b7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="241b7-p103">Запрос страниц по умолчанию возвращает первые 20 страниц, упорядоченные по атрибуту `lastModifiedTime desc`. Если запрос по умолчанию возвращает более 20 страниц, ответ содержит URL-адрес `@odata.nextLink`, который можно использовать для перехода на следующую страницу результатов. Максимальное количество страниц, возвращаемых по запросу `top`, — 100.</span><span class="sxs-lookup"><span data-stu-id="241b7-p103">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="241b7-p104">Ответ по умолчанию разворачивает `parentSection` и выбирает свойства `id`, `displayName` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="241b7-p104">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="241b7-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="241b7-126">Request headers</span></span>
| <span data-ttu-id="241b7-127">Имя</span><span class="sxs-lookup"><span data-stu-id="241b7-127">Name</span></span>       | <span data-ttu-id="241b7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="241b7-128">Type</span></span> | <span data-ttu-id="241b7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="241b7-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="241b7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="241b7-130">Authorization</span></span>  | <span data-ttu-id="241b7-131">string</span><span class="sxs-lookup"><span data-stu-id="241b7-131">string</span></span>  | <span data-ttu-id="241b7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="241b7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="241b7-134">Accept</span><span class="sxs-lookup"><span data-stu-id="241b7-134">Accept</span></span> | <span data-ttu-id="241b7-135">строка</span><span class="sxs-lookup"><span data-stu-id="241b7-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="241b7-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="241b7-136">Request body</span></span>
<span data-ttu-id="241b7-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="241b7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="241b7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="241b7-138">Response</span></span>

<span data-ttu-id="241b7-139">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="241b7-139">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="241b7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="241b7-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="241b7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="241b7-141">Request</span></span>
<span data-ttu-id="241b7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="241b7-142">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="241b7-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="241b7-143">Response</span></span>
<span data-ttu-id="241b7-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="241b7-144">Here is an example of the response.</span></span> <span data-ttu-id="241b7-145">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="241b7-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="241b7-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="241b7-146">All of the properties will be returned from an actual call.</span></span>
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