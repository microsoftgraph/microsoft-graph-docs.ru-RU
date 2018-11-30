---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Восстановление предыдущей версии
ms.openlocfilehash: 507f58e79f209e1e65bfb8dcc2ac666f64a8d45d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076241"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="b9f60-102">Восстановление предыдущей версии ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="b9f60-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="b9f60-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9f60-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9f60-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f60-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9f60-105">Восстановление предыдущей версии ресурса DriveItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="b9f60-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="b9f60-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии файла.</span><span class="sxs-lookup"><span data-stu-id="b9f60-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f60-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f60-107">Permissions</span></span>

<span data-ttu-id="b9f60-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f60-110">Permission type</span></span>      | <span data-ttu-id="b9f60-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f60-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9f60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f60-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f60-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f60-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9f60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f60-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f60-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9f60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f60-116">Application</span></span> | <span data-ttu-id="b9f60-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f60-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f60-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="b9f60-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9f60-119">Request body</span></span>

<span data-ttu-id="b9f60-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="b9f60-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="b9f60-121">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f60-121">Example</span></span>

<span data-ttu-id="b9f60-122">В этом примере восстанавливается версия файла, указанная по `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="b9f60-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="b9f60-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f60-123">Response</span></span>

<span data-ttu-id="b9f60-124">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="b9f60-124">If successful, the API call returns a `204 No content`.</span></span>

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
