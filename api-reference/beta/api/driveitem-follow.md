---
author: chackman
ms.author: chackman
title: ПодПисаться на диск
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 44841c3fec5da5227ddc225d8912a750c1ec3a79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325347"
---
# <a name="follow-drive-item"></a><span data-ttu-id="74ca7-102">ПодПисаться на диск</span><span class="sxs-lookup"><span data-stu-id="74ca7-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ca7-103">ПодПишитесь на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="74ca7-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="74ca7-104">**Примечание:** Чтобы отписаться от элемента, ознакомьтесь со статьей [элемент](driveitem-unfollow.md)не подписаться.</span><span class="sxs-lookup"><span data-stu-id="74ca7-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="74ca7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74ca7-105">Permissions</span></span>

<span data-ttu-id="74ca7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ca7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74ca7-108">Permission type</span></span>      | <span data-ttu-id="74ca7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74ca7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ca7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74ca7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74ca7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="74ca7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74ca7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ca7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ca7-113">Not supported.</span></span>    |
|<span data-ttu-id="74ca7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74ca7-114">Application</span></span> | <span data-ttu-id="74ca7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74ca7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74ca7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="74ca7-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74ca7-117">Request body</span></span>

<span data-ttu-id="74ca7-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="74ca7-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="74ca7-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ca7-119">Response</span></span>

<span data-ttu-id="74ca7-120">Этот метод возвращает объект [DriveItem](../resources/driveitem.md) для отслеживаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="74ca7-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="74ca7-121">Пример</span><span class="sxs-lookup"><span data-stu-id="74ca7-121">Example</span></span>

<span data-ttu-id="74ca7-122">В этом примере используется элемент, `{item-id}`идентифицируемый.</span><span class="sxs-lookup"><span data-stu-id="74ca7-122">This example follows an item identified by `{item-id}`.</span></span>

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
  "suppressions": []
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
