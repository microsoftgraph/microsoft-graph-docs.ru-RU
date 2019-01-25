---
author: chackman
ms.author: chackman
title: Следуйте элемента диска
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0c8835593ed7203cc6239485f1dcd4f17f24fe7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518340"
---
# <a name="follow-drive-item"></a><span data-ttu-id="afbc2-102">Следуйте элемента диска</span><span class="sxs-lookup"><span data-stu-id="afbc2-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afbc2-103">Следуйте [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="afbc2-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="afbc2-104">**Примечание:** Чтобы отменить подписку на элемент, обратитесь к [Unfollow элемента](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="afbc2-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="afbc2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afbc2-105">Permissions</span></span>

<span data-ttu-id="afbc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afbc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afbc2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afbc2-108">Permission type</span></span>      | <span data-ttu-id="afbc2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afbc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afbc2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afbc2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afbc2-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afbc2-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="afbc2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afbc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afbc2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afbc2-113">Not supported.</span></span>    |
|<span data-ttu-id="afbc2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afbc2-114">Application</span></span> | <span data-ttu-id="afbc2-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afbc2-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afbc2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afbc2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="afbc2-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="afbc2-117">Request body</span></span>

<span data-ttu-id="afbc2-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="afbc2-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="afbc2-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="afbc2-119">Response</span></span>

<span data-ttu-id="afbc2-120">Этот метод возвращает [DriveItem](../resources/driveitem.md) для элемента а затем.</span><span class="sxs-lookup"><span data-stu-id="afbc2-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="afbc2-121">Пример</span><span class="sxs-lookup"><span data-stu-id="afbc2-121">Example</span></span>

<span data-ttu-id="afbc2-122">В этом примере исходя из элемента, определяемую средством `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="afbc2-122">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
