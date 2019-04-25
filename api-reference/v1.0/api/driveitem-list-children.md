---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка содержимого папки
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f6e76ca362d8c200ee73b327cdd11ad4b0137e73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548035"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="789d7-102">Создание списка дочерних элементов ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="789d7-102">List children of a driveItem</span></span>

<span data-ttu-id="789d7-103">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="789d7-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="789d7-104">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="789d7-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="789d7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="789d7-105">Permissions</span></span>

<span data-ttu-id="789d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="789d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789d7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="789d7-108">Permission type</span></span>      | <span data-ttu-id="789d7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="789d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="789d7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="789d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="789d7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789d7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="789d7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="789d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="789d7-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789d7-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="789d7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="789d7-114">Application</span></span> | <span data-ttu-id="789d7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789d7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="789d7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="789d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="789d7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="789d7-117">Optional query parameters</span></span>

<span data-ttu-id="789d7-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="789d7-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="789d7-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="789d7-119">Optional request headers</span></span>

| <span data-ttu-id="789d7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="789d7-120">Name</span></span>     | <span data-ttu-id="789d7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="789d7-121">Value</span></span> | <span data-ttu-id="789d7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="789d7-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="789d7-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="789d7-123">_if-none-match_</span></span> | <span data-ttu-id="789d7-124">etag</span><span class="sxs-lookup"><span data-stu-id="789d7-124">etag</span></span>  | <span data-ttu-id="789d7-125">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="789d7-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="789d7-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="789d7-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="789d7-127">Создание списка дочерних элементов в корневой папке диска текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="789d7-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="789d7-128">Чтобы получить файлы, расположенные в корневой папке диска, используйте связь `root` для диска, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="789d7-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="789d7-129">Создание списка дочерних элементов ресурса driveItem с использованием известного идентификатора</span><span class="sxs-lookup"><span data-stu-id="789d7-129">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="789d7-130">Чтобы получить файлы, расположенные в корневой папке диска, используйте связь `root` для диска, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="789d7-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="789d7-131">Создание списка дочерних элементов ресурса driveItem с использованием известного пути</span><span class="sxs-lookup"><span data-stu-id="789d7-131">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="789d7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="789d7-132">Response</span></span>

<span data-ttu-id="789d7-p102">При успешном выполнении этот метод возвращает список элементов в коллекции дочерних элементов для целевого элемента. Коллекция дочерних элементов будет состоять из ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="789d7-p102">If successful, this method returns the list of items in the children collection of the target item. The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="789d7-135">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="789d7-135">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="789d7-136">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="789d7-136">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="789d7-137">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="789d7-137">Error responses</span></span>

<span data-ttu-id="789d7-138">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="789d7-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children"
} -->
