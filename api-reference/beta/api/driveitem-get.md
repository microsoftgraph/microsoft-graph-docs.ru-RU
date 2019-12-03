---
author: JeremyKelley
description: Получение метаданных ресурса DriveItem в объекте Drive по пути в файловой системе или идентификатору.
ms.date: 09/10/2017
title: Получение файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 221a4bd5b9ffaaa7c0b482789b8d663fcf85d470
ms.sourcegitcommit: 6265ddb4e3d22bb556615589594e40df018fb0f1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "39672840"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="f6898-103">Получение ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="f6898-103">Get a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6898-104">Получение метаданных для [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) по пути в файловой системе или идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f6898-104">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6898-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6898-105">Permissions</span></span>

<span data-ttu-id="f6898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6898-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6898-108">Permission type</span></span>      | <span data-ttu-id="f6898-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6898-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6898-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6898-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6898-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span> </br><span data-ttu-id="f6898-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-112">Group.Read.All, Group.ReadWrite.All</span></span> </br><span data-ttu-id="f6898-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-113">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="f6898-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6898-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6898-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6898-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6898-116">Application</span></span> | <span data-ttu-id="f6898-117">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-117">Files.Read.All, Files.ReadWrite.All</span></span> </br><span data-ttu-id="f6898-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-118">Group.Read.All, Group.ReadWrite.All</span></span> </br><span data-ttu-id="f6898-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6898-119">Sites.Read.All, Sites.ReadWrite.All</span></span> |

> <span data-ttu-id="f6898-120">Note: для `/teams` конечной точки требуется использование разрешений Group. Read. ALL или Group. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="f6898-120">Note: The `/teams` endpoint requires the use of Group.Read.All or Group.ReadWrite.All permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6898-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6898-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /teams/{teamId}/channels/{channelId}/filesFolder
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6898-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6898-122">Optional query parameters</span></span>

<span data-ttu-id="f6898-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6898-123">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="f6898-124">С помощью [`$expand`параметра строки запроса](/graph/query-parameters) вы можете включить дочерние элементы запрос на получение метаданных элемента при наличии **дочерней** связи.</span><span class="sxs-lookup"><span data-stu-id="f6898-124">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<span data-ttu-id="f6898-125">Вы также можете использовать параметр `includeDeletedItems=true` запроса, чтобы вернуть удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="f6898-125">You can also use the `includeDeletedItems=true` query parameter to return deleted items.</span></span>
<span data-ttu-id="f6898-126">Этот параметр запроса является допустимым только при нацеливании на [driveItem](../resources/driveitem.md) по идентификатору, и в противном случае он будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="f6898-126">This query parameter is only valid when targeting a [driveItem](../resources/driveitem.md) by ID, and otherwise will be ignored.</span></span>
<span data-ttu-id="f6898-127">В настоящее время поддерживается только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="f6898-127">This is currently only supported on OneDrive Personal.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="f6898-128">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6898-128">Optional request headers</span></span>

| <span data-ttu-id="f6898-129">Имя</span><span class="sxs-lookup"><span data-stu-id="f6898-129">Name</span></span>          | <span data-ttu-id="f6898-130">Значение</span><span class="sxs-lookup"><span data-stu-id="f6898-130">Value</span></span>  | <span data-ttu-id="f6898-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f6898-131">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f6898-132">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f6898-132">if-none-match</span></span> | <span data-ttu-id="f6898-133">String</span><span class="sxs-lookup"><span data-stu-id="f6898-133">String</span></span> | <span data-ttu-id="f6898-134">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f6898-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="f6898-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6898-135">Response</span></span>

<span data-ttu-id="f6898-136">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6898-136">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6898-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f6898-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6898-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6898-138">Request</span></span>

<span data-ttu-id="f6898-139">Ниже приведен пример запроса к корневой папке OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6898-139">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6898-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6898-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```msgraph-interactive
GET /me/drive/root
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6898-141">C#</span><span class="sxs-lookup"><span data-stu-id="f6898-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6898-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6898-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6898-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6898-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

## <a name="response"></a><span data-ttu-id="f6898-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6898-144">Response</span></span>

<span data-ttu-id="f6898-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6898-145">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="f6898-146">Примечания</span><span class="sxs-lookup"><span data-stu-id="f6898-146">Remarks</span></span>

<span data-ttu-id="f6898-147">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="f6898-147">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
}
-->
