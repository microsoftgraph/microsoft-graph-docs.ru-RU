---
title: Получение DriveItemVersion ресурсов
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2924cae410cd7df6a28c7ef81930dee09e566be9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926360"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="59ecf-103">Получение DriveItemVersion ресурсов</span><span class="sxs-lookup"><span data-stu-id="59ecf-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="59ecf-104">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="59ecf-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="59ecf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59ecf-105">Permissions</span></span>

<span data-ttu-id="59ecf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59ecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59ecf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59ecf-108">Permission type</span></span>      | <span data-ttu-id="59ecf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59ecf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59ecf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59ecf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59ecf-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ecf-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59ecf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59ecf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59ecf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ecf-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="59ecf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59ecf-114">Application</span></span> | <span data-ttu-id="59ecf-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59ecf-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="59ecf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59ecf-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="59ecf-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ecf-117">Response</span></span>

<span data-ttu-id="59ecf-118">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59ecf-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="59ecf-119">Пример</span><span class="sxs-lookup"><span data-stu-id="59ecf-119">Example</span></span>

<span data-ttu-id="59ecf-120">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="59ecf-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="59ecf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59ecf-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="59ecf-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ecf-122">Response</span></span>

<span data-ttu-id="59ecf-123">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="59ecf-123">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="59ecf-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="59ecf-124">Remarks</span></span>

<span data-ttu-id="59ecf-125">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="59ecf-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="59ecf-126">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="59ecf-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
