---
title: Восстановление предыдущей версии ресурса DriveItem
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 53a8f5e40e06ef90662a55c44ca718bc82f4fb4b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616254"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="9f720-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="9f720-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="9f720-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="9f720-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="9f720-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="9f720-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f720-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f720-107">Permissions</span></span>

<span data-ttu-id="9f720-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f720-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f720-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f720-110">Permission type</span></span>      | <span data-ttu-id="9f720-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f720-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f720-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f720-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f720-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f720-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f720-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f720-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f720-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f720-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f720-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f720-116">Application</span></span> | <span data-ttu-id="9f720-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f720-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f720-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f720-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="9f720-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f720-119">Request body</span></span>

<span data-ttu-id="9f720-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="9f720-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="9f720-121">Пример</span><span class="sxs-lookup"><span data-stu-id="9f720-121">Example</span></span>

<span data-ttu-id="9f720-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="9f720-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="9f720-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f720-123">Response</span></span>

<span data-ttu-id="9f720-124">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9f720-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f720-125">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9f720-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f720-126">Языках</span><span class="sxs-lookup"><span data-stu-id="9f720-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f720-127">Язык</span><span class="sxs-lookup"><span data-stu-id="9f720-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
