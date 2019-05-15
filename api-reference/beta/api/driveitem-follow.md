---
author: chackman
ms.author: chackman
title: Подписаться на диск
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e62f256e9c4c0832b2f1ef71713c57b596d2a811
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960881"
---
# <a name="follow-drive-item"></a><span data-ttu-id="83e48-102">Подписаться на диск</span><span class="sxs-lookup"><span data-stu-id="83e48-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e48-103">Подпишитесь на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="83e48-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="83e48-104">**Примечание:** Чтобы отписаться от элемента, ознакомьтесь со статьей [элемент](driveitem-unfollow.md)не подписаться.</span><span class="sxs-lookup"><span data-stu-id="83e48-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83e48-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83e48-105">Permissions</span></span>

<span data-ttu-id="83e48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83e48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e48-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83e48-108">Permission type</span></span>      | <span data-ttu-id="83e48-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83e48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83e48-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83e48-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83e48-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e48-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="83e48-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83e48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e48-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83e48-113">Not supported.</span></span>    |
|<span data-ttu-id="83e48-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83e48-114">Application</span></span> | <span data-ttu-id="83e48-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e48-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83e48-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83e48-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="83e48-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83e48-117">Request body</span></span>

<span data-ttu-id="83e48-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="83e48-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="83e48-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="83e48-119">Response</span></span>

<span data-ttu-id="83e48-120">Этот метод возвращает объект [DriveItem](../resources/driveitem.md) для отслеживаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="83e48-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="83e48-121">Пример</span><span class="sxs-lookup"><span data-stu-id="83e48-121">Example</span></span>

<span data-ttu-id="83e48-122">В этом примере используется элемент, `{item-id}`идентифицируемый.</span><span class="sxs-lookup"><span data-stu-id="83e48-122">This example follows an item identified by `{item-id}`.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-follow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="83e48-123">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="83e48-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83e48-124">C#</span><span class="sxs-lookup"><span data-stu-id="83e48-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/follow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83e48-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="83e48-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/follow-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
