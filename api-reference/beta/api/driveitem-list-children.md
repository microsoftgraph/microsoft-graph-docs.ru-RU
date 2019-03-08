---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ПереЧисление содержимого папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 96c5623ba2534086fbcd2130b5b5228e53208c35
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482191"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="e18cf-102">Список дочерних элементов ресурса driveItem.</span><span class="sxs-lookup"><span data-stu-id="e18cf-102">List children of a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e18cf-103">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e18cf-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="e18cf-104">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e18cf-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="e18cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e18cf-105">Permissions</span></span>

<span data-ttu-id="e18cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e18cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e18cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e18cf-108">Permission type</span></span>      | <span data-ttu-id="e18cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e18cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e18cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e18cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e18cf-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18cf-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e18cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e18cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e18cf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18cf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e18cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e18cf-114">Application</span></span> | <span data-ttu-id="e18cf-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18cf-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e18cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e18cf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e18cf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e18cf-117">Optional query parameters</span></span>

<span data-ttu-id="e18cf-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e18cf-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="e18cf-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e18cf-119">Optional request headers</span></span>

| <span data-ttu-id="e18cf-120">Имя заголовка</span><span class="sxs-lookup"><span data-stu-id="e18cf-120">Header name</span></span>     | <span data-ttu-id="e18cf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e18cf-121">Value</span></span> | <span data-ttu-id="e18cf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e18cf-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e18cf-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="e18cf-123">_if-none-match_</span></span> | <span data-ttu-id="e18cf-124">etag</span><span class="sxs-lookup"><span data-stu-id="e18cf-124">etag</span></span>  | <span data-ttu-id="e18cf-125">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом в файле, то будет возвращен отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e18cf-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="e18cf-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="e18cf-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="e18cf-127">Создание списка дочерних элементов в корневой папке объекта drive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="e18cf-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="e18cf-128">Чтобы получить файлы, расположенные в корневой папке объекта drive, используйте связь `root` для drive, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="e18cf-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="e18cf-129">Создание списка дочерних элементов ресурса driveItem с использованием известного идентификатора</span><span class="sxs-lookup"><span data-stu-id="e18cf-129">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="e18cf-130">Чтобы получить файлы, расположенные в корневой папке объекта drive, используйте связь `root` для drive, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="e18cf-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="e18cf-131">Создание списка дочерних элементов ресурса driveItem с использованием известного пути</span><span class="sxs-lookup"><span data-stu-id="e18cf-131">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="e18cf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e18cf-132">Response</span></span>

<span data-ttu-id="e18cf-p102">При успешном выполнении этот метод возвращает список элементов в коллекции дочерних элементов для целевого элемента. Коллекция дочерних элементов будет состоять из ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="e18cf-p102">If successful, this method returns the list of items in the children collection of the target item. The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="e18cf-135">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="e18cf-135">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="e18cf-136">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="e18cf-136">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="e18cf-137">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="e18cf-137">Error responses</span></span>

<span data-ttu-id="e18cf-138">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="e18cf-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
