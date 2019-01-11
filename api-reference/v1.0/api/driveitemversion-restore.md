---
title: Восстановление предыдущей версии ресурса DriveItem
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
localization_priority: Normal
ms.openlocfilehash: 0097d82bb9d317c0bee0392f21040f0963364183
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871612"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="3a12f-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="3a12f-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="3a12f-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="3a12f-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="3a12f-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="3a12f-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a12f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a12f-107">Permissions</span></span>

<span data-ttu-id="3a12f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a12f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a12f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a12f-110">Permission type</span></span>      | <span data-ttu-id="3a12f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a12f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a12f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a12f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a12f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a12f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a12f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a12f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a12f-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a12f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a12f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a12f-116">Application</span></span> | <span data-ttu-id="3a12f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a12f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a12f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a12f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="3a12f-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a12f-119">Request body</span></span>

<span data-ttu-id="3a12f-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="3a12f-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="3a12f-121">Пример</span><span class="sxs-lookup"><span data-stu-id="3a12f-121">Example</span></span>

<span data-ttu-id="3a12f-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="3a12f-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="3a12f-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a12f-123">Response</span></span>

<span data-ttu-id="3a12f-124">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a12f-124">If successful, the API call returns a `204 No Content`.</span></span>

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
