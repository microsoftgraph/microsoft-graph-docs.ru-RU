---
author: chackman
description: Подпишитесь на driveItem.
title: Подписаться на диск
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9056e385a8231afc20669d22542a41fb680da3dd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416823"
---
# <a name="follow-drive-item"></a><span data-ttu-id="58e10-103">Подписаться на диск</span><span class="sxs-lookup"><span data-stu-id="58e10-103">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e10-104">Подпишитесь на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="58e10-104">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="58e10-105">**Примечание:** Чтобы отписаться от элемента, ознакомьтесь со статьей [элемент](driveitem-unfollow.md)не подписаться.</span><span class="sxs-lookup"><span data-stu-id="58e10-105">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58e10-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58e10-106">Permissions</span></span>

<span data-ttu-id="58e10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e10-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e10-109">Permission type</span></span>      | <span data-ttu-id="58e10-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e10-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e10-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e10-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58e10-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e10-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58e10-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e10-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e10-114">Not supported.</span></span>    |
|<span data-ttu-id="58e10-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58e10-115">Application</span></span> | <span data-ttu-id="58e10-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e10-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e10-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e10-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="58e10-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58e10-118">Request body</span></span>

<span data-ttu-id="58e10-119">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="58e10-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="58e10-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e10-120">Response</span></span>

<span data-ttu-id="58e10-121">Этот метод возвращает объект [DriveItem](../resources/driveitem.md) для отслеживаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="58e10-121">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="58e10-122">Пример</span><span class="sxs-lookup"><span data-stu-id="58e10-122">Example</span></span>

<span data-ttu-id="58e10-123">В этом примере используется элемент, `{item-id}`идентифицируемый.</span><span class="sxs-lookup"><span data-stu-id="58e10-123">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58e10-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="58e10-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58e10-125">C#</span><span class="sxs-lookup"><span data-stu-id="58e10-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58e10-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58e10-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58e10-127">Цель — C</span><span class="sxs-lookup"><span data-stu-id="58e10-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
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
