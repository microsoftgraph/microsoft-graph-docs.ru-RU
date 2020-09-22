---
title: Список страниц
description: Получение списка объектов Page из указанного раздела.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ac6b6547481cccb5baa9b03bebab2d92fd34d410
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074108"
---
# <a name="list-pages"></a><span data-ttu-id="85980-103">Список страниц</span><span class="sxs-lookup"><span data-stu-id="85980-103">List pages</span></span>

<span data-ttu-id="85980-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85980-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85980-105">Получение списка объектов [Page](../resources/onenotepage.md) из указанного раздела.</span><span class="sxs-lookup"><span data-stu-id="85980-105">Retrieve a list of [page](../resources/onenotepage.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="85980-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85980-106">Permissions</span></span>
<span data-ttu-id="85980-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85980-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85980-109">Permission type</span></span>      | <span data-ttu-id="85980-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85980-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85980-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85980-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85980-112">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85980-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="85980-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85980-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85980-114">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85980-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="85980-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85980-115">Application</span></span> | <span data-ttu-id="85980-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85980-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85980-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85980-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85980-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85980-118">Optional query parameters</span></span>
<span data-ttu-id="85980-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85980-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="85980-120">Запрос по умолчанию для страниц возвращает 20 первых страниц, упорядоченных по `lastModifiedTime desc` .</span><span class="sxs-lookup"><span data-stu-id="85980-120">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`.</span></span> <span data-ttu-id="85980-121">Если запрос по умолчанию возвращает более 20 страниц, ответ содержит элемент `@odata.nextLink` , который можно использовать для страницы в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="85980-121">If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set.</span></span> <span data-ttu-id="85980-122">Максимальное количество страниц, возвращаемых для `top` запроса — 100.</span><span class="sxs-lookup"><span data-stu-id="85980-122">The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="85980-123">Ответ по умолчанию разворачивается `parentSection` и выбирает `id` Свойства раздела, `name` а также `self` Свойства.</span><span class="sxs-lookup"><span data-stu-id="85980-123">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="85980-124">Допустимые `expand` значения для страниц: `parentNotebook` и `parentSection` .</span><span class="sxs-lookup"><span data-stu-id="85980-124">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85980-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85980-125">Request headers</span></span>
| <span data-ttu-id="85980-126">Имя</span><span class="sxs-lookup"><span data-stu-id="85980-126">Name</span></span>       | <span data-ttu-id="85980-127">Тип</span><span class="sxs-lookup"><span data-stu-id="85980-127">Type</span></span> | <span data-ttu-id="85980-128">Описание</span><span class="sxs-lookup"><span data-stu-id="85980-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="85980-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="85980-129">Authorization</span></span>  | <span data-ttu-id="85980-130">string</span><span class="sxs-lookup"><span data-stu-id="85980-130">string</span></span>  | <span data-ttu-id="85980-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85980-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85980-133">Accept</span><span class="sxs-lookup"><span data-stu-id="85980-133">Accept</span></span> | <span data-ttu-id="85980-134">строка</span><span class="sxs-lookup"><span data-stu-id="85980-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="85980-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85980-135">Request body</span></span>
<span data-ttu-id="85980-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85980-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85980-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="85980-137">Response</span></span>

<span data-ttu-id="85980-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [оненотепаже](../resources/onenotepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85980-138">If successful, this method returns a `200 OK` response code and a collection of [onenotePage](../resources/onenotepage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85980-139">Пример</span><span class="sxs-lookup"><span data-stu-id="85980-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85980-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="85980-140">Request</span></span>
<span data-ttu-id="85980-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85980-141">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="85980-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="85980-142">Response</span></span>
<span data-ttu-id="85980-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85980-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
<!--
{
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


