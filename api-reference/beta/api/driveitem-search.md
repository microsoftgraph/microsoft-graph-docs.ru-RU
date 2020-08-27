---
author: JeremyKelley
description: Поиск элементов, соответствующих запросу, в иерархии элементов.
ms.date: 09/10/2017
title: Поиск файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: edd6a0f1c43b7aa27b4089a63902840ce7e2562d
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287472"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="76fa3-103">Поиск элементов DriveItem на диске</span><span class="sxs-lookup"><span data-stu-id="76fa3-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="76fa3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76fa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76fa3-105">Поиск элементов, соответствующих запросу, в иерархии элементов.</span><span class="sxs-lookup"><span data-stu-id="76fa3-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="76fa3-106">Вы можете выполнить поиск в иерархии папок, на всем диске или среди файлов, к которым предоставлен доступ текущему пользователю.</span><span class="sxs-lookup"><span data-stu-id="76fa3-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="76fa3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76fa3-107">Permissions</span></span>

<span data-ttu-id="76fa3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76fa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76fa3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76fa3-110">Permission type</span></span>      | <span data-ttu-id="76fa3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76fa3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76fa3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76fa3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76fa3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76fa3-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="76fa3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76fa3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76fa3-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76fa3-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="76fa3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76fa3-116">Application</span></span> | <span data-ttu-id="76fa3-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76fa3-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76fa3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76fa3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76fa3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76fa3-119">Optional query parameters</span></span>

<span data-ttu-id="76fa3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76fa3-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="76fa3-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="76fa3-121">Function parameters</span></span>

| <span data-ttu-id="76fa3-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="76fa3-122">Parameter</span></span> | <span data-ttu-id="76fa3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="76fa3-123">Type</span></span>  | <span data-ttu-id="76fa3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="76fa3-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="76fa3-125">q</span><span class="sxs-lookup"><span data-stu-id="76fa3-125">q</span></span>  | <span data-ttu-id="76fa3-126">string</span><span class="sxs-lookup"><span data-stu-id="76fa3-126">string</span></span> | <span data-ttu-id="76fa3-p103">Текст запроса, используемый для поиска элементов. Для поиска можно использовать несколько полей, включая поля имени файла, метаданных и содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="76fa3-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="76fa3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="76fa3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="76fa3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="76fa3-130">Request</span></span>

<span data-ttu-id="76fa3-131">В примере ниже выполняется поиск совпадения для запроса "Проект Contoso" в нескольких полях элементов диска пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="76fa3-131">The following example searches for a match for "Contoso Project" across several fields in the signed-in user's drive items.</span></span>

# <a name="http"></a>[<span data-ttu-id="76fa3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="76fa3-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search" }-->

```msgraph-interactive
GET /me/drive/root/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="76fa3-133">C#</span><span class="sxs-lookup"><span data-stu-id="76fa3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76fa3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76fa3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76fa3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76fa3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76fa3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="76fa3-136">Response</span></span>

<span data-ttu-id="76fa3-p104">Этот метод возвращает объект, который содержит коллекцию элементов [DriveItem](../resources/driveitem.md), соответствующих условиям поиска. Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="76fa3-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="76fa3-p105">Если будет найдено слишком много совпадений, отклик будет разбит на страницы, а свойство **@odata.nextLink** будет содержать URL-адрес на следующую страницу с результатами. Чтобы указать количество элементов на странице, вы можете использовать параметр запроса `$top`.</span><span class="sxs-lookup"><span data-stu-id="76fa3-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="76fa3-141">Поиск элементов, к которым пользователь может получить доступ</span><span class="sxs-lookup"><span data-stu-id="76fa3-141">Searching for items a user can access</span></span>

<span data-ttu-id="76fa3-p106">Помимо поиска элементов на диске ваше приложение может выполнять более широкий поиск и включать элементы, к которым текущему пользователю предоставлен доступ. Чтобы расширить область поиска, используйте метод **search** в ресурсе [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="76fa3-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="76fa3-144">Пример</span><span class="sxs-lookup"><span data-stu-id="76fa3-144">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="76fa3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="76fa3-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all" }-->

```msgraph-interactive
GET /me/drive/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="76fa3-146">C#</span><span class="sxs-lookup"><span data-stu-id="76fa3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76fa3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76fa3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76fa3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76fa3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76fa3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="76fa3-149">Response</span></span>

<span data-ttu-id="76fa3-p107">Отклики при поиске на ресурсе **Drive** могут включать элементы, расположенные за пределами диска (элементы, к которым текущему пользователю предоставлен доступ). Эти элементы будут содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что они хранятся не на целевом диске.</span><span class="sxs-lookup"><span data-stu-id="76fa3-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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

## <a name="error-responses"></a><span data-ttu-id="76fa3-152">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="76fa3-152">Error responses</span></span>

<span data-ttu-id="76fa3-153">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="76fa3-153">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
