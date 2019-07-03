---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 43d46caf83a028b751a0c21c3bffe69ee0983c11
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436188"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="0af0e-102">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="0af0e-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af0e-103">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="0af0e-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="0af0e-104">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="0af0e-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="0af0e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0af0e-105">Permissions</span></span>

<span data-ttu-id="0af0e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af0e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0af0e-108">Permission type</span></span>      | <span data-ttu-id="0af0e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0af0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af0e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0af0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0af0e-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af0e-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0af0e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0af0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af0e-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af0e-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0af0e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0af0e-114">Application</span></span> | <span data-ttu-id="0af0e-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af0e-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0af0e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0af0e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="0af0e-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0af0e-117">Request body</span></span>

<span data-ttu-id="0af0e-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="0af0e-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="0af0e-119">Пример</span><span class="sxs-lookup"><span data-stu-id="0af0e-119">Example</span></span>

<span data-ttu-id="0af0e-120">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="0af0e-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0af0e-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af0e-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0af0e-122">C#</span><span class="sxs-lookup"><span data-stu-id="0af0e-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0af0e-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="0af0e-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0af0e-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0af0e-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="0af0e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af0e-125">Response</span></span>

<span data-ttu-id="0af0e-126">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0af0e-126">If successful, the API call returns a `204 No content`.</span></span>

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
