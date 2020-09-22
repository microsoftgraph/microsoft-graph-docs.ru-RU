---
title: Вывод страницы
description: Получение свойств и связей объекта Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 3ab71087bcbed6b75c4f14f285c46ee56bf9f2ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086993"
---
# <a name="get-page"></a><span data-ttu-id="f213e-103">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="f213e-103">Get page</span></span>

<span data-ttu-id="f213e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f213e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f213e-105">Получение свойств и связей объекта [Page](../resources/page.md) .</span><span class="sxs-lookup"><span data-stu-id="f213e-105">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="f213e-106">**Извлечение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="f213e-106">**Getting page information**</span></span>

<span data-ttu-id="f213e-107">Доступ к метаданным страницы по идентификатору страницы:</span><span class="sxs-lookup"><span data-stu-id="f213e-107">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="f213e-108">**Извлечение контента страницы**</span><span class="sxs-lookup"><span data-stu-id="f213e-108">**Getting page content**</span></span>

<span data-ttu-id="f213e-109">Вы можете использовать `content` конечную точку страницы для получения HTML-содержимого страницы:</span><span class="sxs-lookup"><span data-stu-id="f213e-109">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="f213e-110">`includeIDs=true`Параметр запроса используется для [обновления страниц](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="f213e-110">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f213e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f213e-111">Permissions</span></span>
<span data-ttu-id="f213e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f213e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f213e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f213e-114">Permission type</span></span>      | <span data-ttu-id="f213e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f213e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f213e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f213e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f213e-117">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f213e-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f213e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f213e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f213e-119">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f213e-119">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f213e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f213e-120">Application</span></span> | <span data-ttu-id="f213e-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f213e-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f213e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f213e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f213e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f213e-123">Optional query parameters</span></span>
<span data-ttu-id="f213e-124">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f213e-124">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f213e-125">Ответ по умолчанию разворачивается `parentSection` и выбирает `id` Свойства раздела, `name` а также `self` Свойства.</span><span class="sxs-lookup"><span data-stu-id="f213e-125">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="f213e-126">Допустимые `expand` значения для страниц: `parentNotebook` и `parentSection` .</span><span class="sxs-lookup"><span data-stu-id="f213e-126">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f213e-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f213e-127">Request headers</span></span>
| <span data-ttu-id="f213e-128">Имя</span><span class="sxs-lookup"><span data-stu-id="f213e-128">Name</span></span>       | <span data-ttu-id="f213e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f213e-129">Type</span></span> | <span data-ttu-id="f213e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f213e-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f213e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f213e-131">Authorization</span></span>  | <span data-ttu-id="f213e-132">string</span><span class="sxs-lookup"><span data-stu-id="f213e-132">string</span></span>  | <span data-ttu-id="f213e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f213e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f213e-135">Accept</span><span class="sxs-lookup"><span data-stu-id="f213e-135">Accept</span></span> | <span data-ttu-id="f213e-136">строка</span><span class="sxs-lookup"><span data-stu-id="f213e-136">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f213e-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f213e-137">Request body</span></span>
<span data-ttu-id="f213e-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f213e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f213e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f213e-139">Response</span></span>

<span data-ttu-id="f213e-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Page](../resources/page.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f213e-140">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f213e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f213e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f213e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f213e-142">Request</span></span>
<span data-ttu-id="f213e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f213e-143">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="f213e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f213e-144">Response</span></span>
<span data-ttu-id="f213e-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f213e-145">Here is an example of the response.</span></span> <span data-ttu-id="f213e-146">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="f213e-146">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="f213e-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f213e-147">All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

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

