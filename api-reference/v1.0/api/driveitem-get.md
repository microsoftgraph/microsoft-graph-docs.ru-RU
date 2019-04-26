---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение файла или папки
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9cff51558f84556fc05c69164ba48809acc12fa8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548028"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="987aa-102">Получение ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="987aa-102">Get a DriveItem resource</span></span>

<span data-ttu-id="987aa-103">Получение метаданных для [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) по пути в файловой системе или идентификатору.</span><span class="sxs-lookup"><span data-stu-id="987aa-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="987aa-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="987aa-104">Permissions</span></span>

<span data-ttu-id="987aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="987aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="987aa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="987aa-107">Permission type</span></span>      | <span data-ttu-id="987aa-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="987aa-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="987aa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="987aa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="987aa-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987aa-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="987aa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="987aa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="987aa-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987aa-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="987aa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="987aa-113">Application</span></span> | <span data-ttu-id="987aa-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987aa-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="987aa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="987aa-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="987aa-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="987aa-116">Optional query parameters</span></span>

<span data-ttu-id="987aa-117">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="987aa-117">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="987aa-118">С помощью [`$expand`параметра строки запроса](/graph/query-parameters) вы можете включить дочерние элементы запрос на получение метаданных элемента при наличии **дочерней** связи.</span><span class="sxs-lookup"><span data-stu-id="987aa-118">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="987aa-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="987aa-119">Optional request headers</span></span>

| <span data-ttu-id="987aa-120">Имя</span><span class="sxs-lookup"><span data-stu-id="987aa-120">Name</span></span>          | <span data-ttu-id="987aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="987aa-121">Value</span></span>  | <span data-ttu-id="987aa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="987aa-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="987aa-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="987aa-123">if-none-match</span></span> | <span data-ttu-id="987aa-124">String</span><span class="sxs-lookup"><span data-stu-id="987aa-124">String</span></span> | <span data-ttu-id="987aa-125">Если указан этот заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то будет возвращен ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="987aa-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="987aa-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="987aa-126">Response</span></span>

<span data-ttu-id="987aa-127">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="987aa-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="987aa-128">Пример</span><span class="sxs-lookup"><span data-stu-id="987aa-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="987aa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="987aa-129">Request</span></span>

<span data-ttu-id="987aa-130">Ниже приведен пример запроса к корневой папке OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="987aa-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="987aa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="987aa-131">Response</span></span>

<span data-ttu-id="987aa-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="987aa-132">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="987aa-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="987aa-133">Remarks</span></span>

<span data-ttu-id="987aa-134">Дополнительные сведения о возвращении ошибок см. в статье об [ответах с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="987aa-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
