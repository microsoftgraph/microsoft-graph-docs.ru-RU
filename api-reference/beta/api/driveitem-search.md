---
author: JeremyKelley
description: Поиск элементов, соответствующих запросу, в иерархии элементов.
ms.date: 09/10/2017
title: Поиск файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 26a34f5b8ca8a0d0897cba3f3b9cada0b65107c6
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719327"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="e399c-103">Поиск элементов DriveItem на диске</span><span class="sxs-lookup"><span data-stu-id="e399c-103">Search for a DriveItems within a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e399c-104">Поиск элементов, соответствующих запросу, в иерархии элементов.</span><span class="sxs-lookup"><span data-stu-id="e399c-104">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="e399c-105">Вы можете выполнить поиск в иерархии папок, на всем диске или среди файлов, к которым предоставлен доступ текущему пользователю.</span><span class="sxs-lookup"><span data-stu-id="e399c-105">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="e399c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e399c-106">Permissions</span></span>

<span data-ttu-id="e399c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e399c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e399c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e399c-109">Permission type</span></span>      | <span data-ttu-id="e399c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e399c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e399c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e399c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e399c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e399c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e399c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e399c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e399c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e399c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e399c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e399c-115">Application</span></span> | <span data-ttu-id="e399c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e399c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e399c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e399c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e399c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e399c-118">Optional query parameters</span></span>

<span data-ttu-id="e399c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e399c-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="e399c-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e399c-120">Function parameters</span></span>

| <span data-ttu-id="e399c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="e399c-121">Parameter</span></span> | <span data-ttu-id="e399c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e399c-122">Type</span></span>  | <span data-ttu-id="e399c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e399c-123">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e399c-124">q</span><span class="sxs-lookup"><span data-stu-id="e399c-124">q</span></span>  | <span data-ttu-id="e399c-125">string</span><span class="sxs-lookup"><span data-stu-id="e399c-125">string</span></span> | <span data-ttu-id="e399c-p103">Текст запроса, используемый для поиска элементов. Для поиска можно использовать несколько полей, включая поля имени файла, метаданных и содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="e399c-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="e399c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e399c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e399c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e399c-129">Request</span></span>

<span data-ttu-id="e399c-130">Вот пример запроса, выполняющего поиск в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e399c-130">Here is an example of the request searching the current user's OneDrive</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e399c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e399c-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search" }-->

```msgraph-interactive
GET /me/drive/root/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e399c-132">C#</span><span class="sxs-lookup"><span data-stu-id="e399c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e399c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e399c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e399c-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e399c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e399c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e399c-135">Response</span></span>

<span data-ttu-id="e399c-p104">Этот метод возвращает объект, который содержит коллекцию элементов [DriveItem](../resources/driveitem.md), соответствующих условиям поиска. Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="e399c-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="e399c-p105">Если будет найдено слишком много совпадений, отклик будет разбит на страницы, а свойство **@odata.nextLink** будет содержать URL-адрес на следующую страницу с результатами. Чтобы указать количество элементов на странице, вы можете использовать параметр запроса `$top`.</span><span class="sxs-lookup"><span data-stu-id="e399c-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="e399c-140">Поиск элементов, к которым пользователь может получить доступ</span><span class="sxs-lookup"><span data-stu-id="e399c-140">Searching for items a user can access</span></span>

<span data-ttu-id="e399c-p106">Помимо поиска элементов на диске ваше приложение может выполнять более широкий поиск и включать элементы, к которым текущему пользователю предоставлен доступ. Чтобы расширить область поиска, используйте метод **search** в ресурсе [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="e399c-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="e399c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e399c-143">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e399c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e399c-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all" }-->

```msgraph-interactive
GET /me/drive/search(q='{search-query}')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e399c-145">C#</span><span class="sxs-lookup"><span data-stu-id="e399c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e399c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e399c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e399c-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e399c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e399c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e399c-148">Response</span></span>

<span data-ttu-id="e399c-p107">Отклики при поиске на ресурсе **Drive** могут включать элементы, расположенные за пределами диска (элементы, к которым текущему пользователю предоставлен доступ). Эти элементы будут содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что они хранятся не на целевом диске.</span><span class="sxs-lookup"><span data-stu-id="e399c-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="e399c-151">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="e399c-151">Error responses</span></span>

<span data-ttu-id="e399c-152">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="e399c-152">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
}
-->
