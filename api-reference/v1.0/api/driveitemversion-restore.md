---
title: Восстановление предыдущей версии ресурса DriveItem
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: ac2b2ac3b734071f8537e149034788999a983f15
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806186"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="ea230-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="ea230-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="ea230-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea230-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea230-106">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="ea230-106">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="ea230-107">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="ea230-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea230-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea230-108">Permissions</span></span>

<span data-ttu-id="ea230-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea230-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea230-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea230-111">Permission type</span></span>      | <span data-ttu-id="ea230-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea230-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea230-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea230-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea230-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea230-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea230-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea230-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea230-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea230-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea230-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea230-117">Application</span></span> | <span data-ttu-id="ea230-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea230-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea230-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea230-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="ea230-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea230-120">Request body</span></span>

<span data-ttu-id="ea230-121">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="ea230-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="ea230-122">Пример</span><span class="sxs-lookup"><span data-stu-id="ea230-122">Example</span></span>

<span data-ttu-id="ea230-123">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="ea230-123">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea230-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea230-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="ea230-125">C#</span><span class="sxs-lookup"><span data-stu-id="ea230-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea230-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea230-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea230-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea230-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea230-128">Java</span><span class="sxs-lookup"><span data-stu-id="ea230-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ea230-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea230-129">Response</span></span>

<span data-ttu-id="ea230-130">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea230-130">If successful, the API call returns a `204 No Content`.</span></span>

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
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
