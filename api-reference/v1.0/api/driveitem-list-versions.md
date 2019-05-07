---
title: Перечисление версий объекта DriveItem
description: OneDrive и SharePoint можно настроить на хранение журнала для файлов.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: afd73c26c8a35cbac7c66397c89b1a9466af5971
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616106"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="0c3a1-103">Перечисление версий объекта DriveItem</span><span class="sxs-lookup"><span data-stu-id="0c3a1-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="0c3a1-104">OneDrive и SharePoint можно настроить на хранение журнала для файлов.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="0c3a1-105">В зависимости от того, каковы служба и конфигурация, новую версию можно создавать при каждом изменении или сохранении, создавать вручную или не создавать никогда.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="0c3a1-106">Предыдущие версии документа могут храниться в течение ограниченного времени в зависимости от того, каковы параметры администратора, которые могут быть уникальными для каждого пользователя или расположения.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c3a1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c3a1-107">Permissions</span></span>

<span data-ttu-id="0c3a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c3a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c3a1-110">Permission type</span></span>      | <span data-ttu-id="0c3a1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c3a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c3a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c3a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c3a1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3a1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c3a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c3a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c3a1-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3a1-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c3a1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c3a1-116">Application</span></span> | <span data-ttu-id="0c3a1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3a1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="0c3a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c3a1-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="0c3a1-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c3a1-119">Response</span></span>

<span data-ttu-id="0c3a1-120">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="0c3a1-121">Пример</span><span class="sxs-lookup"><span data-stu-id="0c3a1-121">Example</span></span>

<span data-ttu-id="0c3a1-122">В этом примере показано, как получить версии файла для объекта Drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c3a1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c3a1-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="0c3a1-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c3a1-124">Response</span></span>

<span data-ttu-id="0c3a1-125">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="0c3a1-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c3a1-126">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0c3a1-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c3a1-127">Языках</span><span class="sxs-lookup"><span data-stu-id="0c3a1-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-previous-versions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c3a1-128">Язык</span><span class="sxs-lookup"><span data-stu-id="0c3a1-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-previous-versions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="0c3a1-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="0c3a1-129">Remarks</span></span>

<span data-ttu-id="0c3a1-130">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-130">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="0c3a1-131">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="0c3a1-131">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
