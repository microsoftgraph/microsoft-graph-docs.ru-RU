---
title: Восстановление предыдущей версии ресурса DriveItem
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
ms.openlocfilehash: e8272678e048391279d5b2147985d4f1e83f0456
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027797"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="d405a-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="d405a-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="d405a-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="d405a-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="d405a-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="d405a-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="d405a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d405a-107">Permissions</span></span>

<span data-ttu-id="d405a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d405a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d405a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d405a-110">Permission type</span></span>      | <span data-ttu-id="d405a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d405a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d405a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d405a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d405a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d405a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d405a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d405a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d405a-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d405a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d405a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d405a-116">Application</span></span> | <span data-ttu-id="d405a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d405a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d405a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d405a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="d405a-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d405a-119">Request body</span></span>

<span data-ttu-id="d405a-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="d405a-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="d405a-121">Пример</span><span class="sxs-lookup"><span data-stu-id="d405a-121">Example</span></span>

<span data-ttu-id="d405a-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="d405a-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="d405a-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="d405a-123">Response</span></span>

<span data-ttu-id="d405a-124">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d405a-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
