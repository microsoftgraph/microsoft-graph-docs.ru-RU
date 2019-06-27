---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ede7eb6275a4d23c715a3c981686355fc20aa369
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259950"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="8331c-102">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="8331c-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8331c-103">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="8331c-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="8331c-104">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="8331c-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="8331c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8331c-105">Permissions</span></span>

<span data-ttu-id="8331c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8331c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8331c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8331c-108">Permission type</span></span>      | <span data-ttu-id="8331c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8331c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8331c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8331c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8331c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8331c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8331c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8331c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8331c-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8331c-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8331c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8331c-114">Application</span></span> | <span data-ttu-id="8331c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8331c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8331c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8331c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="8331c-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8331c-117">Request body</span></span>

<span data-ttu-id="8331c-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="8331c-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="8331c-119">Пример</span><span class="sxs-lookup"><span data-stu-id="8331c-119">Example</span></span>

<span data-ttu-id="8331c-120">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="8331c-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="8331c-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="8331c-121">Response</span></span>

<span data-ttu-id="8331c-122">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="8331c-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8331c-123">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8331c-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8331c-124">C#</span><span class="sxs-lookup"><span data-stu-id="8331c-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8331c-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="8331c-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8331c-126">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8331c-126">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/restore-item-version-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
