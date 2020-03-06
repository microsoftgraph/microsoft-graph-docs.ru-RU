---
title: Получение ресурса DriveItemVersion
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 0d2ae9ca2e742ab7a9d7338be12e57ec4033e2a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517645"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="ed721-103">Получение ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="ed721-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="ed721-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed721-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed721-105">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ed721-105">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed721-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed721-106">Permissions</span></span>

<span data-ttu-id="ed721-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed721-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed721-109">Permission type</span></span>      | <span data-ttu-id="ed721-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed721-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed721-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed721-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed721-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed721-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed721-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed721-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed721-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed721-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed721-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed721-115">Application</span></span> | <span data-ttu-id="ed721-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed721-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ed721-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed721-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="ed721-118">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed721-118">Response</span></span>

<span data-ttu-id="ed721-119">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ed721-119">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ed721-120">Пример</span><span class="sxs-lookup"><span data-stu-id="ed721-120">Example</span></span>

<span data-ttu-id="ed721-121">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ed721-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ed721-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed721-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed721-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed721-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}
```
# <a name="c"></a>[<span data-ttu-id="ed721-124">C#</span><span class="sxs-lookup"><span data-stu-id="ed721-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed721-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed721-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed721-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed721-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed721-127">Java</span><span class="sxs-lookup"><span data-stu-id="ed721-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed721-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed721-128">Response</span></span>

<span data-ttu-id="ed721-129">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="ed721-129">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="ed721-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="ed721-130">Remarks</span></span>

<span data-ttu-id="ed721-131">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="ed721-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ed721-132">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="ed721-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
