---
title: Вывод страницы
description: Получение свойств и связей объекта Page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 963aeeec95b9c57dbb0a024aeca2afdfba16a9d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556447"
---
# <a name="get-page"></a><span data-ttu-id="8af2f-103">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="8af2f-103">Get page</span></span>

<span data-ttu-id="8af2f-104">Получение свойств и связей объекта [Page](../resources/page.md) .</span><span class="sxs-lookup"><span data-stu-id="8af2f-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="8af2f-105">**Извлечение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="8af2f-105">**Getting page information**</span></span>

<span data-ttu-id="8af2f-106">Доступ к метаданным страницы по идентификатору страницы:</span><span class="sxs-lookup"><span data-stu-id="8af2f-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="8af2f-107">**Извлечение контента страницы**</span><span class="sxs-lookup"><span data-stu-id="8af2f-107">**Getting page content**</span></span>

<span data-ttu-id="8af2f-108">Вы можете использовать `content` конечную точку страницы для получения HTML-содержимого страницы:</span><span class="sxs-lookup"><span data-stu-id="8af2f-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="8af2f-109">Параметр `includeIDs=true` запроса используется для [обновления страниц](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="8af2f-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8af2f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8af2f-110">Permissions</span></span>
<span data-ttu-id="8af2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af2f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8af2f-113">Permission type</span></span>      | <span data-ttu-id="8af2f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8af2f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8af2f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8af2f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8af2f-116">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8af2f-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8af2f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8af2f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8af2f-118">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8af2f-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8af2f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8af2f-119">Application</span></span> | <span data-ttu-id="8af2f-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af2f-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8af2f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8af2f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8af2f-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8af2f-122">Optional query parameters</span></span>
<span data-ttu-id="8af2f-123">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8af2f-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8af2f-124">`parentSection` Ответ по умолчанию разворачивается и выбирает свойства `id`раздела `name`, а `self` также свойства.</span><span class="sxs-lookup"><span data-stu-id="8af2f-124">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties.</span></span> <span data-ttu-id="8af2f-125">Допустимые `expand` значения для страниц `parentNotebook` : `parentSection`и.</span><span class="sxs-lookup"><span data-stu-id="8af2f-125">Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8af2f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8af2f-126">Request headers</span></span>
| <span data-ttu-id="8af2f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="8af2f-127">Name</span></span>       | <span data-ttu-id="8af2f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8af2f-128">Type</span></span> | <span data-ttu-id="8af2f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8af2f-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8af2f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8af2f-130">Authorization</span></span>  | <span data-ttu-id="8af2f-131">string</span><span class="sxs-lookup"><span data-stu-id="8af2f-131">string</span></span>  | <span data-ttu-id="8af2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8af2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8af2f-134">Accept</span><span class="sxs-lookup"><span data-stu-id="8af2f-134">Accept</span></span> | <span data-ttu-id="8af2f-135">string</span><span class="sxs-lookup"><span data-stu-id="8af2f-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8af2f-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8af2f-136">Request body</span></span>
<span data-ttu-id="8af2f-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8af2f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af2f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8af2f-138">Response</span></span>

<span data-ttu-id="8af2f-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Page](../resources/page.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8af2f-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8af2f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8af2f-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8af2f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8af2f-141">Request</span></span>
<span data-ttu-id="8af2f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8af2f-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="8af2f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8af2f-143">Response</span></span>
<span data-ttu-id="8af2f-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8af2f-144">Here is an example of the response.</span></span> <span data-ttu-id="8af2f-145">Note: объект Response, показанный здесь, усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="8af2f-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="8af2f-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8af2f-146">All of the properties will be returned from an actual call.</span></span>
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
