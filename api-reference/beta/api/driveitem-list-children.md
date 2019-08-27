---
author: JeremyKelley
description: Возвращает коллекцию DriveItems в дочерних элементах ресурса DriveItem.
ms.date: 09/10/2017
title: Создание списка содержимого папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 91945814dab0ab8793620d413fc0610560253741
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633288"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="c1f4d-103">Создание списка дочерних элементов ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="c1f4d-103">List children of a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1f4d-104">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-104">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="c1f4d-105">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-105">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="c1f4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1f4d-106">Permissions</span></span>

<span data-ttu-id="c1f4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1f4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1f4d-109">Permission type</span></span>      | <span data-ttu-id="c1f4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1f4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1f4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1f4d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1f4d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f4d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1f4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1f4d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1f4d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f4d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1f4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1f4d-115">Application</span></span> | <span data-ttu-id="c1f4d-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f4d-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1f4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1f4d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1f4d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1f4d-118">Optional query parameters</span></span>

<span data-ttu-id="c1f4d-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-119">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="c1f4d-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1f4d-120">Optional request headers</span></span>

| <span data-ttu-id="c1f4d-121">Имя заголовка</span><span class="sxs-lookup"><span data-stu-id="c1f4d-121">Header name</span></span>     | <span data-ttu-id="c1f4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1f4d-122">Value</span></span> | <span data-ttu-id="c1f4d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c1f4d-123">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c1f4d-124">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="c1f4d-124">_if-none-match_</span></span> | <span data-ttu-id="c1f4d-125">etag</span><span class="sxs-lookup"><span data-stu-id="c1f4d-125">etag</span></span>  | <span data-ttu-id="c1f4d-126">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="c1f4d-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1f4d-127">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="c1f4d-128">Создание списка дочерних элементов в корневой папке диска текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="c1f4d-128">List children in the root of the current user's drive</span></span>

<span data-ttu-id="c1f4d-129">Чтобы получить файлы, расположенные в корневой папке объекта drive, используйте связь `root` для drive, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-129">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c1f4d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1f4d-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1f4d-131">C#</span><span class="sxs-lookup"><span data-stu-id="c1f4d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1f4d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1f4d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1f4d-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1f4d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="c1f4d-134">Создание списка дочерних элементов ресурса driveItem с использованием известного идентификатора</span><span class="sxs-lookup"><span data-stu-id="c1f4d-134">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="c1f4d-135">Чтобы получить файлы, расположенные в корневой папке диска, используйте связь `root` для диска, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-135">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c1f4d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1f4d-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1f4d-137">C#</span><span class="sxs-lookup"><span data-stu-id="c1f4d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1f4d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1f4d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1f4d-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1f4d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="c1f4d-140">Создание списка дочерних элементов ресурса driveItem с использованием известного пути</span><span class="sxs-lookup"><span data-stu-id="c1f4d-140">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="c1f4d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1f4d-141">Response</span></span>

<span data-ttu-id="c1f4d-142">При успешном выполнении этот метод возвращает список элементов в коллекции дочерних элементов для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-142">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="c1f4d-143">Коллекция дочерних элементов будет состоять из ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="c1f4d-143">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="c1f4d-144">**Примечание:** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство \*\* \@OData. nextLink\*\* возвращается в ответе, чтобы указать, что доступны дополнительные элементы, и укажите URL-адрес запроса для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="c1f4d-144">**Note:** If a collection exceeds the default page size (200 items), the **\@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="c1f4d-145">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="c1f4d-145">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="c1f4d-146">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="c1f4d-146">Error responses</span></span>

<span data-ttu-id="c1f4d-147">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="c1f4d-147">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
}
-->
