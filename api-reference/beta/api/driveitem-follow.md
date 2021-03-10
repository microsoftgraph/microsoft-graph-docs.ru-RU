---
author: chackman
description: Отслеживание ресурса driveItem.
title: Следуйте элементу диска
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8294ded183dcd6dfea7d2b3c9f16b18c5412d316
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625873"
---
# <a name="follow-drive-item"></a><span data-ttu-id="c2a58-103">Следуйте элементу диска</span><span class="sxs-lookup"><span data-stu-id="c2a58-103">Follow drive item</span></span>

<span data-ttu-id="c2a58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2a58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2a58-105">Следуйте [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c2a58-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="c2a58-106">**Примечание:** Чтобы отоблести элемент, см. [в статье Unfollow item](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="c2a58-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2a58-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2a58-107">Permissions</span></span>

<span data-ttu-id="c2a58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2a58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2a58-110">Permission type</span></span>      | <span data-ttu-id="c2a58-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2a58-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2a58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2a58-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2a58-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a58-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2a58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2a58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2a58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2a58-115">Not supported.</span></span>    |
|<span data-ttu-id="c2a58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2a58-116">Application</span></span> | <span data-ttu-id="c2a58-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a58-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2a58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2a58-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id}/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="c2a58-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2a58-119">Request body</span></span>

<span data-ttu-id="c2a58-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="c2a58-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="c2a58-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2a58-121">Response</span></span>

<span data-ttu-id="c2a58-122">Этот метод возвращает [driveItem для](../resources/driveitem.md) элемента, за которым следует.</span><span class="sxs-lookup"><span data-stu-id="c2a58-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="c2a58-123">Пример</span><span class="sxs-lookup"><span data-stu-id="c2a58-123">Example</span></span>

<span data-ttu-id="c2a58-124">В этом примере следует элемент, идентифицированный `{item-id}` .</span><span class="sxs-lookup"><span data-stu-id="c2a58-124">This example follows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2a58-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2a58-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="c"></a>[<span data-ttu-id="c2a58-126">C#</span><span class="sxs-lookup"><span data-stu-id="c2a58-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2a58-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2a58-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2a58-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2a58-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2a58-129">Java</span><span class="sxs-lookup"><span data-stu-id="c2a58-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-item-java-snippets.md)]
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


