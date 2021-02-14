---
author: JeremyKelley
ms.date: 09/10/2017
title: Получение файла или папки
localization_priority: Priority
ms.prod: sharepoint
description: Получение метаданных ресурса DriveItem в объекте Drive по пути в файловой системе или идентификатору.
doc_type: apiPageType
ms.openlocfilehash: 7fb47cd473114d5ecd376c092584b7166d6801eb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240306"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="f7238-103">Получение ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="f7238-103">Get a DriveItem resource</span></span>

<span data-ttu-id="f7238-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7238-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7238-105">Получение метаданных для [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) по пути в файловой системе или идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f7238-105">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7238-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7238-106">Permissions</span></span>

<span data-ttu-id="f7238-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7238-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7238-109">Permission type</span></span>      | <span data-ttu-id="f7238-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7238-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7238-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7238-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7238-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7238-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7238-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7238-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7238-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7238-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7238-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7238-115">Application</span></span> | <span data-ttu-id="f7238-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7238-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7238-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7238-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{site-id}/drive/items/{item-id}
GET /sites/{site-id}/drive/root:/{item-path}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/driveItem
GET /users/{user-id}/drive/items/{item-id}
GET /users/{user-id}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7238-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7238-118">Optional query parameters</span></span>

<span data-ttu-id="f7238-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f7238-119">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="f7238-120">С помощью [`$expand`параметра строки запроса](/graph/query-parameters) вы можете включить дочерние элементы запрос на получение метаданных элемента при наличии **дочерней** связи.</span><span class="sxs-lookup"><span data-stu-id="f7238-120">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<span data-ttu-id="f7238-121">Чтобы вернуть удаленные элементы, можно также использовать параметр запроса `includeDeletedItems=true`.</span><span class="sxs-lookup"><span data-stu-id="f7238-121">You can also use the `includeDeletedItems=true` query parameter to return deleted items.</span></span>
<span data-ttu-id="f7238-122">Этот параметр запроса действителен только тогда, когда целевым объектом назначается [driveItem](../resources/driveitem.md) через идентификатор, в ином случае он игнорируется.</span><span class="sxs-lookup"><span data-stu-id="f7238-122">This query parameter is only valid when targeting a [driveItem](../resources/driveitem.md) by ID, and otherwise will be ignored.</span></span>
<span data-ttu-id="f7238-123">В настоящее время этот параметр поддерживается только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="f7238-123">This is currently only supported on OneDrive Personal.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="f7238-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7238-124">Optional request headers</span></span>

| <span data-ttu-id="f7238-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f7238-125">Name</span></span>          | <span data-ttu-id="f7238-126">Значение</span><span class="sxs-lookup"><span data-stu-id="f7238-126">Value</span></span>  | <span data-ttu-id="f7238-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f7238-127">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f7238-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f7238-128">if-none-match</span></span> | <span data-ttu-id="f7238-129">String</span><span class="sxs-lookup"><span data-stu-id="f7238-129">String</span></span> | <span data-ttu-id="f7238-130">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f7238-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="f7238-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7238-131">Response</span></span>

<span data-ttu-id="f7238-132">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7238-132">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7238-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f7238-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7238-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7238-134">Request</span></span>

<span data-ttu-id="f7238-135">Ниже приведен пример запроса к корневой папке OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7238-135">Here is an example of the request to the root folder of the user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7238-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7238-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/root
```
# <a name="c"></a>[<span data-ttu-id="f7238-137">C#</span><span class="sxs-lookup"><span data-stu-id="f7238-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7238-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7238-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7238-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7238-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7238-140">Java</span><span class="sxs-lookup"><span data-stu-id="f7238-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f7238-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7238-141">Response</span></span>

<span data-ttu-id="f7238-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7238-142">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a><span data-ttu-id="f7238-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="f7238-143">Remarks</span></span>

<span data-ttu-id="f7238-144">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="f7238-144">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
} -->

