---
author: chackman
ms.author: chackman
title: Подписаться на диск
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1dc7cdd1f863687773236fee927b6c5a37cf82ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436426"
---
# <a name="follow-drive-item"></a><span data-ttu-id="3c9fa-102">Подписаться на диск</span><span class="sxs-lookup"><span data-stu-id="3c9fa-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c9fa-103">Подпишитесь на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c9fa-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="3c9fa-104">**Примечание:** Чтобы отписаться от элемента, ознакомьтесь со статьей [элемент](driveitem-unfollow.md)не подписаться.</span><span class="sxs-lookup"><span data-stu-id="3c9fa-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c9fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c9fa-105">Permissions</span></span>

<span data-ttu-id="3c9fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c9fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c9fa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c9fa-108">Permission type</span></span>      | <span data-ttu-id="3c9fa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c9fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c9fa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c9fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c9fa-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9fa-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c9fa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c9fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c9fa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c9fa-113">Not supported.</span></span>    |
|<span data-ttu-id="3c9fa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c9fa-114">Application</span></span> | <span data-ttu-id="3c9fa-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9fa-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c9fa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c9fa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="3c9fa-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c9fa-117">Request body</span></span>

<span data-ttu-id="3c9fa-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="3c9fa-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="3c9fa-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c9fa-119">Response</span></span>

<span data-ttu-id="3c9fa-120">Этот метод возвращает объект [DriveItem](../resources/driveitem.md) для отслеживаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="3c9fa-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="3c9fa-121">Пример</span><span class="sxs-lookup"><span data-stu-id="3c9fa-121">Example</span></span>

<span data-ttu-id="3c9fa-122">В этом примере используется элемент, `{item-id}`идентифицируемый.</span><span class="sxs-lookup"><span data-stu-id="3c9fa-122">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c9fa-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c9fa-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c9fa-124">C#</span><span class="sxs-lookup"><span data-stu-id="3c9fa-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c9fa-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c9fa-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c9fa-126">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c9fa-126">Objective-C</span></span>](#tab/objc)
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
