---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Создание списка содержимого папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 982bb2374d02ee48408d8c500041fad7813b8588
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951217"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="7f20c-102">Создание списка дочерних элементов ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="7f20c-102">List children of a driveItem</span></span>

> <span data-ttu-id="7f20c-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f20c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f20c-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f20c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f20c-105">Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="7f20c-105">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="7f20c-106">Ресурсы DriveItem с аспектом **папки** или **пакета**, отличным от NULL, могут содержать один или несколько дочерних элементов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="7f20c-106">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="7f20c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f20c-107">Permissions</span></span>

<span data-ttu-id="7f20c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f20c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f20c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f20c-110">Permission type</span></span>      | <span data-ttu-id="7f20c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f20c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f20c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f20c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f20c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f20c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f20c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f20c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f20c-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f20c-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f20c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f20c-116">Application</span></span> | <span data-ttu-id="7f20c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f20c-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f20c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f20c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f20c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f20c-119">Optional query parameters</span></span>

<span data-ttu-id="7f20c-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7f20c-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="7f20c-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f20c-121">Optional request headers</span></span>

| <span data-ttu-id="7f20c-122">Имя заголовка</span><span class="sxs-lookup"><span data-stu-id="7f20c-122">Header name</span></span>     | <span data-ttu-id="7f20c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7f20c-123">Value</span></span> | <span data-ttu-id="7f20c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7f20c-124">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7f20c-125">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="7f20c-125">_if-none-match_</span></span> | <span data-ttu-id="7f20c-126">etag</span><span class="sxs-lookup"><span data-stu-id="7f20c-126">etag</span></span>  | <span data-ttu-id="7f20c-127">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="7f20c-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="7f20c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7f20c-128">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="7f20c-129">Создание списка дочерних элементов в корневой папке объекта drive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="7f20c-129">List children in the root of the current user's drive</span></span>

<span data-ttu-id="7f20c-130">Чтобы получить файлы, расположенные в корневой папке объекта drive, используйте связь `root` для drive, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="7f20c-130">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="7f20c-131">Создание списка дочерних элементов ресурса driveItem с использованием известного идентификатора</span><span class="sxs-lookup"><span data-stu-id="7f20c-131">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="7f20c-132">Чтобы получить файлы, расположенные в корневой папке объекта drive, используйте связь `root` для drive, а затем получите доступ к связи дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="7f20c-132">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="7f20c-133">Создание списка дочерних элементов ресурса driveItem с использованием известного пути</span><span class="sxs-lookup"><span data-stu-id="7f20c-133">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="7f20c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f20c-134">Response</span></span>

<span data-ttu-id="7f20c-135">При успешном выполнении этот метод возвращает список элементов в коллекции дочерних элементов для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="7f20c-135">If successful, this method returns the list of items in the children collection of the target item.</span></span>
<span data-ttu-id="7f20c-136">Коллекция дочерних элементов будет состоять из ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="7f20c-136">The children collection will be composed of [driveItem][item-resource] resources.</span></span>

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

<span data-ttu-id="7f20c-137">**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.</span><span class="sxs-lookup"><span data-stu-id="7f20c-137">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="7f20c-138">Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span><span class="sxs-lookup"><span data-stu-id="7f20c-138">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="7f20c-139">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="7f20c-139">Error responses</span></span>

<span data-ttu-id="7f20c-140">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="7f20c-140">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children"
} -->
