---
author: JeremyKelley
description: Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 73c5f590976dc8b6f2e529421449895bb1863f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956907"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="356b6-104">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="356b6-104">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356b6-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="356b6-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="356b6-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="356b6-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="356b6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="356b6-107">Permissions</span></span>

<span data-ttu-id="356b6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="356b6-110">Permission type</span></span>      | <span data-ttu-id="356b6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="356b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="356b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="356b6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356b6-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="356b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="356b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356b6-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356b6-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="356b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="356b6-116">Application</span></span> | <span data-ttu-id="356b6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356b6-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="356b6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="356b6-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="356b6-119">Request body</span></span>

<span data-ttu-id="356b6-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="356b6-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="356b6-121">Пример</span><span class="sxs-lookup"><span data-stu-id="356b6-121">Example</span></span>

<span data-ttu-id="356b6-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="356b6-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="356b6-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="356b6-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="356b6-124">C#</span><span class="sxs-lookup"><span data-stu-id="356b6-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="356b6-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="356b6-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="356b6-126">Цель — C</span><span class="sxs-lookup"><span data-stu-id="356b6-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="356b6-127">Java</span><span class="sxs-lookup"><span data-stu-id="356b6-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="356b6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="356b6-128">Response</span></span>

<span data-ttu-id="356b6-129">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="356b6-129">If successful, the API call returns a `204 No content`.</span></span>

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
