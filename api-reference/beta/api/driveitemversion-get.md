---
title: Получение ресурса DriveItemVersion (ознакомительная версия)
description: В этой статье рассказывается, как получить метаданные для определенной версии ресурса DriveItem.
ms.openlocfilehash: c78a81d1a5428bbb969f8761b238655ab7919e5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076614"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="48f37-103">Получение ресурса DriveItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="48f37-103">Get a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="48f37-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48f37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48f37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48f37-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48f37-106">В этой статье рассказывается, как получить метаданные для определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="48f37-106">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48f37-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48f37-107">Permissions</span></span>

<span data-ttu-id="48f37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48f37-110">Permission type</span></span>      | <span data-ttu-id="48f37-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48f37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48f37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48f37-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48f37-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f37-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="48f37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48f37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f37-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f37-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="48f37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48f37-116">Application</span></span> | <span data-ttu-id="48f37-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f37-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="48f37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48f37-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="48f37-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="48f37-119">Response</span></span>

<span data-ttu-id="48f37-120">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [DriveItemVersion](../resources/driveitemversion.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48f37-120">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="48f37-121">Пример</span><span class="sxs-lookup"><span data-stu-id="48f37-121">Example</span></span>

<span data-ttu-id="48f37-122">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="48f37-122">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="48f37-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48f37-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="48f37-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="48f37-124">Response</span></span>

<span data-ttu-id="48f37-125">Возвращается коллекция версий:</span><span class="sxs-lookup"><span data-stu-id="48f37-125">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="48f37-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="48f37-126">Remarks</span></span>

<span data-ttu-id="48f37-127">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="48f37-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="48f37-128">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="48f37-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
