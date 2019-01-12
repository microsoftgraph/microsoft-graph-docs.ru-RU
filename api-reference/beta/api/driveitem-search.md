---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Поиск файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ee1d8f6ba1c22426beb70d9ad89650e48e6900ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959694"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="89ece-102">Поиск элементов DriveItem на диске</span><span class="sxs-lookup"><span data-stu-id="89ece-102">Search for a DriveItems within a drive</span></span>

> <span data-ttu-id="89ece-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89ece-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89ece-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ece-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89ece-105">Поиск элементов, соответствующих запросу, в иерархии элементов.</span><span class="sxs-lookup"><span data-stu-id="89ece-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="89ece-106">Вы можете выполнить поиск в иерархии папок, в объекте drive или среди файлов, к которым предоставлен доступ текущему пользователю.</span><span class="sxs-lookup"><span data-stu-id="89ece-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ece-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89ece-107">Permissions</span></span>

<span data-ttu-id="89ece-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ece-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ece-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89ece-110">Permission type</span></span>      | <span data-ttu-id="89ece-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89ece-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ece-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89ece-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89ece-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ece-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="89ece-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89ece-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ece-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ece-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="89ece-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89ece-116">Application</span></span> | <span data-ttu-id="89ece-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ece-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ece-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89ece-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89ece-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89ece-119">Optional query parameters</span></span>

<span data-ttu-id="89ece-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="89ece-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="89ece-121">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="89ece-121">Function parameters</span></span>

| <span data-ttu-id="89ece-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="89ece-122">Parameter</span></span> | <span data-ttu-id="89ece-123">Тип</span><span class="sxs-lookup"><span data-stu-id="89ece-123">Type</span></span>  | <span data-ttu-id="89ece-124">Описание</span><span class="sxs-lookup"><span data-stu-id="89ece-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="89ece-125">q</span><span class="sxs-lookup"><span data-stu-id="89ece-125">q</span></span>  | <span data-ttu-id="89ece-126">string</span><span class="sxs-lookup"><span data-stu-id="89ece-126">string</span></span> | <span data-ttu-id="89ece-p104">Текст запроса, используемый для поиска элементов. Для поиска можно использовать несколько полей, включая поля имени файла, метаданных и содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="89ece-p104">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="89ece-129">Пример</span><span class="sxs-lookup"><span data-stu-id="89ece-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ece-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="89ece-130">Request</span></span>

<span data-ttu-id="89ece-131">Вот пример запроса, выполняющего поиск в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="89ece-131">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="89ece-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ece-132">Response</span></span>

<span data-ttu-id="89ece-p105">Этот метод возвращает объект, который содержит коллекцию элементов [DriveItem](../resources/driveitem.md), соответствующих условиям поиска. Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="89ece-p105">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="89ece-p106">Если будет найдено слишком много совпадений, отклик будет разбит на страницы, а свойство **@odata.nextLink** будет содержать URL-адрес на следующую страницу с результатами. Чтобы указать количество элементов на странице, вы можете использовать параметр запроса `$top`.</span><span class="sxs-lookup"><span data-stu-id="89ece-p106">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="89ece-137">Поиск элементов, к которым пользователь может получить доступ</span><span class="sxs-lookup"><span data-stu-id="89ece-137">Searching for items a user can access</span></span>

<span data-ttu-id="89ece-p107">Помимо поиска элементов на диске ваше приложение может выполнять более широкий поиск и включать элементы, к которым текущему пользователю предоставлен доступ. Чтобы расширить область поиска, используйте метод **search** в ресурсе [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="89ece-p107">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="89ece-140">Пример</span><span class="sxs-lookup"><span data-stu-id="89ece-140">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="89ece-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ece-141">Response</span></span>

<span data-ttu-id="89ece-p108">Отклики при поиске на ресурсе **Drive** могут включать элементы, расположенные за пределами диска (элементы, к которым текущему пользователю предоставлен доступ). Эти элементы будут содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что они хранятся не на целевом диске.</span><span class="sxs-lookup"><span data-stu-id="89ece-p108">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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

## <a name="error-responses"></a><span data-ttu-id="89ece-144">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="89ece-144">Error responses</span></span>

<span data-ttu-id="89ece-145">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="89ece-145">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search"
} -->
