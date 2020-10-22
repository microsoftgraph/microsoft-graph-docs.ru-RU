---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка содержимого папки
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции ресурсов DriveItem, являющихся дочерними элементами ресурса DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 6afe3475b0e213ba0906a46838ae09ec95ebc9b6
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634496"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="d89d8-103">Создание списка дочерних элементов ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="d89d8-103">List children of a driveItem</span></span>

<span data-ttu-id="d89d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d89d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d89d8-105">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="d89d8-105">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="d89d8-106">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="d89d8-106">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="d89d8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d89d8-107">Permissions</span></span>

<span data-ttu-id="d89d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d89d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d89d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d89d8-110">Permission type</span></span>      | <span data-ttu-id="d89d8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d89d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d89d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d89d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d89d8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89d8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d89d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d89d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d89d8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89d8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d89d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d89d8-116">Application</span></span> | <span data-ttu-id="d89d8-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89d8-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d89d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d89d8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d89d8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d89d8-119">Optional query parameters</span></span>

<span data-ttu-id="d89d8-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d89d8-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="d89d8-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d89d8-121">Optional request headers</span></span>

| <span data-ttu-id="d89d8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d89d8-122">Name</span></span>     | <span data-ttu-id="d89d8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d89d8-123">Value</span></span> | <span data-ttu-id="d89d8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d89d8-124">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d89d8-125">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="d89d8-125">_if-none-match_</span></span> | <span data-ttu-id="d89d8-126">etag</span><span class="sxs-lookup"><span data-stu-id="d89d8-126">etag</span></span>  | <span data-ttu-id="d89d8-127">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d89d8-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="d89d8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d89d8-128">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="d89d8-129">Создание списка дочерних элементов в корневой папке диска текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="d89d8-129">List children in the root of the current user's drive</span></span>

<span data-ttu-id="d89d8-130">Чтобы получить файлы, расположенные в корневой папке диска, используйте связь `root` для диска, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="d89d8-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="http"></a>[<span data-ttu-id="d89d8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d89d8-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/root/children
```
# <a name="c"></a>[<span data-ttu-id="d89d8-132">C#</span><span class="sxs-lookup"><span data-stu-id="d89d8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d89d8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d89d8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d89d8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d89d8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d89d8-135">Java</span><span class="sxs-lookup"><span data-stu-id="d89d8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="d89d8-136">Создание списка дочерних элементов ресурса driveItem с использованием известного идентификатора</span><span class="sxs-lookup"><span data-stu-id="d89d8-136">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="d89d8-137">Чтобы получить файлы, расположенные в корневой папке диска, используйте связь `root` для диска, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="d89d8-137">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>


# <a name="http"></a>[<span data-ttu-id="d89d8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d89d8-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-children-files", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/children
```
# <a name="c"></a>[<span data-ttu-id="d89d8-139">C#</span><span class="sxs-lookup"><span data-stu-id="d89d8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-children-files-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d89d8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d89d8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-children-files-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d89d8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d89d8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-children-files-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d89d8-142">Java</span><span class="sxs-lookup"><span data-stu-id="d89d8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-children-files-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="d89d8-143">Создание списка дочерних элементов ресурса driveItem с использованием известного пути</span><span class="sxs-lookup"><span data-stu-id="d89d8-143">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="d89d8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d89d8-144">Response</span></span>

<span data-ttu-id="d89d8-145">При успешном выполнении этот метод возвращает список элементов в коллекции дочерних элементов для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="d89d8-145">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="d89d8-146">Коллекция дочерних элементов будет состоять из ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="d89d8-146">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children-files", "list-children-from-path" ] } -->

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

<span data-ttu-id="d89d8-147">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **\@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="d89d8-147">**Note:** If a collection exceeds the default page size (200 items), the **\@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="d89d8-148">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="d89d8-148">You can control the page size through [optional query string parameters](/graph/query-parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="d89d8-149">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="d89d8-149">Error responses</span></span>

<span data-ttu-id="d89d8-150">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="d89d8-150">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
  ]
} -->
