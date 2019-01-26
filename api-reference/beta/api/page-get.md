---
title: Получение страницы
description: Получение свойств и связей объекта page.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 1cafa1b430f20fc74d045c498d7bba81eb160463
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572635"
---
# <a name="get-page"></a><span data-ttu-id="1dae7-103">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="1dae7-103">Get page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dae7-104">Получение свойств и связей объекта [page](../resources/onenotepage.md).</span><span class="sxs-lookup"><span data-stu-id="1dae7-104">Retrieve the properties and relationships of a [page](../resources/onenotepage.md) object.</span></span>

<span data-ttu-id="1dae7-105">**Получение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="1dae7-105">**Getting page information**</span></span>

<span data-ttu-id="1dae7-106">Доступ к метаданным страницы по ее идентификатору:</span><span class="sxs-lookup"><span data-stu-id="1dae7-106">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="1dae7-107">**Получение содержимого страницы**</span><span class="sxs-lookup"><span data-stu-id="1dae7-107">**Getting page content**</span></span>

<span data-ttu-id="1dae7-108">Чтобы получить содержимое HTML страницы, вы можете использовать конечную точку `content` страницы:</span><span class="sxs-lookup"><span data-stu-id="1dae7-108">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="1dae7-109">Параметр запроса `includeIDs=true` используется для [обновления страниц](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="1dae7-109">The `includeIDs=true` query option is used to [update pages](../api/page-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dae7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dae7-110">Permissions</span></span>
<span data-ttu-id="1dae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dae7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dae7-113">Permission type</span></span>      | <span data-ttu-id="1dae7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dae7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dae7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dae7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1dae7-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dae7-116">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1dae7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dae7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dae7-118">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dae7-118">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1dae7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dae7-119">Application</span></span> | <span data-ttu-id="1dae7-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dae7-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dae7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dae7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1dae7-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1dae7-122">Optional query parameters</span></span>
<span data-ttu-id="1dae7-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1dae7-123">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1dae7-p102">Отклик, возвращаемый по умолчанию, разворачивает `parentSection` и выбирает свойства `id`, `name` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="1dae7-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dae7-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dae7-126">Request headers</span></span>
| <span data-ttu-id="1dae7-127">Имя</span><span class="sxs-lookup"><span data-stu-id="1dae7-127">Name</span></span>       | <span data-ttu-id="1dae7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1dae7-128">Type</span></span> | <span data-ttu-id="1dae7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1dae7-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1dae7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dae7-130">Authorization</span></span>  | <span data-ttu-id="1dae7-131">string</span><span class="sxs-lookup"><span data-stu-id="1dae7-131">string</span></span>  | <span data-ttu-id="1dae7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dae7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dae7-134">Accept</span><span class="sxs-lookup"><span data-stu-id="1dae7-134">Accept</span></span> | <span data-ttu-id="1dae7-135">строка</span><span class="sxs-lookup"><span data-stu-id="1dae7-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1dae7-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dae7-136">Request body</span></span>
<span data-ttu-id="1dae7-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dae7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dae7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dae7-138">Response</span></span>

<span data-ttu-id="1dae7-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [page](../resources/onenotepage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dae7-139">If successful, this method returns a `200 OK` response code and the [page](../resources/onenotepage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dae7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1dae7-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dae7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dae7-141">Request</span></span>
<span data-ttu-id="1dae7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dae7-142">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="1dae7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dae7-143">Response</span></span>
<span data-ttu-id="1dae7-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1dae7-144">Here is an example of the response.</span></span> <span data-ttu-id="1dae7-145">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="1dae7-145">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="1dae7-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dae7-146">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
