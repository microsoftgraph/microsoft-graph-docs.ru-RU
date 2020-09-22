---
author: JeremyKelley
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ca944b58941ae9951510dcea5edcb8dcda751efd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981823"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="6fae2-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="6fae2-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="6fae2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fae2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fae2-106">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="6fae2-106">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="6fae2-107">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="6fae2-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fae2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fae2-108">Permissions</span></span>

<span data-ttu-id="6fae2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fae2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fae2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fae2-111">Permission type</span></span>      | <span data-ttu-id="6fae2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fae2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fae2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fae2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6fae2-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fae2-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fae2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fae2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fae2-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fae2-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fae2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fae2-117">Application</span></span> | <span data-ttu-id="6fae2-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fae2-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fae2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fae2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="6fae2-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fae2-120">Request body</span></span>

<span data-ttu-id="6fae2-121">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="6fae2-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="6fae2-122">Пример</span><span class="sxs-lookup"><span data-stu-id="6fae2-122">Example</span></span>

<span data-ttu-id="6fae2-123">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="6fae2-123">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="6fae2-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fae2-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="6fae2-125">C#</span><span class="sxs-lookup"><span data-stu-id="6fae2-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fae2-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fae2-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fae2-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fae2-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6fae2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fae2-128">Response</span></span>

<span data-ttu-id="6fae2-129">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="6fae2-129">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->


