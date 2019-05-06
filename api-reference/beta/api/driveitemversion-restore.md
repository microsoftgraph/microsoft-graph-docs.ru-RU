---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e04a46804e5963695e2bd1ee0356e3e754d36ccd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588136"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="f015a-102">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="f015a-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f015a-103">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="f015a-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="f015a-104">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="f015a-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="f015a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f015a-105">Permissions</span></span>

<span data-ttu-id="f015a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f015a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f015a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f015a-108">Permission type</span></span>      | <span data-ttu-id="f015a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f015a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f015a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f015a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f015a-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f015a-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f015a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f015a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f015a-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f015a-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f015a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f015a-114">Application</span></span> | <span data-ttu-id="f015a-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f015a-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f015a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f015a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="f015a-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f015a-117">Request body</span></span>

<span data-ttu-id="f015a-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="f015a-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f015a-119">Пример</span><span class="sxs-lookup"><span data-stu-id="f015a-119">Example</span></span>

<span data-ttu-id="f015a-120">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="f015a-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="f015a-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="f015a-121">Response</span></span>

<span data-ttu-id="f015a-122">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="f015a-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f015a-123">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f015a-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f015a-124">Языках</span><span class="sxs-lookup"><span data-stu-id="f015a-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f015a-125">Язык</span><span class="sxs-lookup"><span data-stu-id="f015a-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
