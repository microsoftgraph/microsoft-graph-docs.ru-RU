---
title: Получение ресурса DriveItemVersion
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 783090c9ec98d3df04b6a4b1595626132ddca768
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616147"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="87651-103">Получение ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="87651-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="87651-104">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="87651-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87651-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87651-105">Permissions</span></span>

<span data-ttu-id="87651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87651-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87651-108">Permission type</span></span>      | <span data-ttu-id="87651-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87651-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87651-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87651-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87651-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87651-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87651-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87651-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87651-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87651-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="87651-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87651-114">Application</span></span> | <span data-ttu-id="87651-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87651-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="87651-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87651-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="87651-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="87651-117">Response</span></span>

<span data-ttu-id="87651-118">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87651-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="87651-119">Пример</span><span class="sxs-lookup"><span data-stu-id="87651-119">Example</span></span>

<span data-ttu-id="87651-120">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="87651-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="87651-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87651-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="87651-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="87651-122">Response</span></span>

<span data-ttu-id="87651-123">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="87651-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="87651-124">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="87651-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="87651-125">Языках</span><span class="sxs-lookup"><span data-stu-id="87651-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87651-126">Язык</span><span class="sxs-lookup"><span data-stu-id="87651-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="87651-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="87651-127">Remarks</span></span>

<span data-ttu-id="87651-128">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="87651-128">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="87651-129">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="87651-129">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
