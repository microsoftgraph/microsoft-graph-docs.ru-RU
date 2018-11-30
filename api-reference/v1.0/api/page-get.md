---
title: Получение страницы
description: Получение свойств и связей объекта page.
ms.openlocfilehash: a1715547152afd2c3ef73eecd1a285d7b1d3806a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027000"
---
# <a name="get-page"></a><span data-ttu-id="5102d-103">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="5102d-103">Get page</span></span>

<span data-ttu-id="5102d-104">Получение свойств и связей объекта [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="5102d-104">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="5102d-105">**Получение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="5102d-105">**Getting page information**</span></span>

<span data-ttu-id="5102d-106">Доступ к метаданным страницы по ее идентификатору:</span><span class="sxs-lookup"><span data-stu-id="5102d-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="5102d-107">**Получение содержимого страницы**</span><span class="sxs-lookup"><span data-stu-id="5102d-107">**Getting page content**</span></span>

<span data-ttu-id="5102d-108">Чтобы получить содержимое HTML страницы, вы можете использовать конечную точку `content` страницы:</span><span class="sxs-lookup"><span data-stu-id="5102d-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="5102d-109">Параметр запроса `includeIDs=true` используется для [обновления страниц](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="5102d-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5102d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5102d-110">Permissions</span></span>
<span data-ttu-id="5102d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5102d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5102d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5102d-113">Permission type</span></span>      | <span data-ttu-id="5102d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5102d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5102d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5102d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5102d-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5102d-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5102d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5102d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5102d-118">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5102d-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5102d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5102d-119">Application</span></span> | <span data-ttu-id="5102d-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5102d-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5102d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5102d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5102d-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5102d-122">Optional query parameters</span></span>
<span data-ttu-id="5102d-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5102d-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5102d-p102">Отклик, возвращаемый по умолчанию, разворачивает `parentSection` и выбирает свойства `id`, `name` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="5102d-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5102d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5102d-126">Request headers</span></span>
| <span data-ttu-id="5102d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="5102d-127">Name</span></span>       | <span data-ttu-id="5102d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5102d-128">Type</span></span> | <span data-ttu-id="5102d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5102d-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5102d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5102d-130">Authorization</span></span>  | <span data-ttu-id="5102d-131">string</span><span class="sxs-lookup"><span data-stu-id="5102d-131">string</span></span>  | <span data-ttu-id="5102d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5102d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5102d-134">Accept</span><span class="sxs-lookup"><span data-stu-id="5102d-134">Accept</span></span> | <span data-ttu-id="5102d-135">строка</span><span class="sxs-lookup"><span data-stu-id="5102d-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5102d-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5102d-136">Request body</span></span>
<span data-ttu-id="5102d-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5102d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5102d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5102d-138">Response</span></span>

<span data-ttu-id="5102d-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [page](../resources/page.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5102d-139">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5102d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="5102d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5102d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5102d-141">Request</span></span>
<span data-ttu-id="5102d-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5102d-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="5102d-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="5102d-143">Response</span></span>
<span data-ttu-id="5102d-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5102d-144">Here is an example of the response.</span></span> <span data-ttu-id="5102d-145">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5102d-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="5102d-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5102d-146">All of the properties will be returned from an actual call.</span></span>
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
