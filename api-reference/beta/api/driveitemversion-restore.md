---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Восстановление предыдущей версии
localization_priority: Normal
ms.openlocfilehash: 6b325edc637779327390f34d6ebaab7dee2666cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813883"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="7b1d2-102">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="7b1d2-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="7b1d2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b1d2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b1d2-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="7b1d2-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b1d2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b1d2-107">Permissions</span></span>

<span data-ttu-id="7b1d2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b1d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b1d2-110">Permission type</span></span>      | <span data-ttu-id="7b1d2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b1d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b1d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b1d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b1d2-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b1d2-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b1d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b1d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b1d2-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b1d2-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b1d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b1d2-116">Application</span></span> | <span data-ttu-id="7b1d2-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b1d2-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b1d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b1d2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="7b1d2-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b1d2-119">Request body</span></span>

<span data-ttu-id="7b1d2-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="7b1d2-121">Пример</span><span class="sxs-lookup"><span data-stu-id="7b1d2-121">Example</span></span>

<span data-ttu-id="7b1d2-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="7b1d2-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b1d2-123">Response</span></span>

<span data-ttu-id="7b1d2-124">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="7b1d2-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
