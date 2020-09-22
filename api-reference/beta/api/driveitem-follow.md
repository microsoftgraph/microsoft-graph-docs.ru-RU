---
author: chackman
description: Отслеживание ресурса driveItem.
title: Подписаться на диск
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c509d2a08d819e814754f3d835624ebaed7f754a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982061"
---
# <a name="follow-drive-item"></a><span data-ttu-id="fe958-103">Подписаться на диск</span><span class="sxs-lookup"><span data-stu-id="fe958-103">Follow drive item</span></span>

<span data-ttu-id="fe958-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe958-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe958-105">Подпишитесь на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="fe958-106">**Примечание:** Чтобы отписаться от элемента, ознакомьтесь со статьей [элемент не подписаться](driveitem-unfollow.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe958-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe958-107">Permissions</span></span>

<span data-ttu-id="fe958-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe958-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe958-110">Permission type</span></span>      | <span data-ttu-id="fe958-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe958-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe958-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe958-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe958-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe958-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe958-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe958-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe958-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe958-115">Not supported.</span></span>    |
|<span data-ttu-id="fe958-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe958-116">Application</span></span> | <span data-ttu-id="fe958-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe958-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe958-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe958-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="fe958-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe958-119">Request body</span></span>

<span data-ttu-id="fe958-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="fe958-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="fe958-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe958-121">Response</span></span>

<span data-ttu-id="fe958-122">Этот метод возвращает объект [DriveItem](../resources/driveitem.md) для отслеживаемого элемента.</span><span class="sxs-lookup"><span data-stu-id="fe958-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="fe958-123">Пример</span><span class="sxs-lookup"><span data-stu-id="fe958-123">Example</span></span>

<span data-ttu-id="fe958-124">В этом примере используется элемент, идентифицируемый `{item-id}` .</span><span class="sxs-lookup"><span data-stu-id="fe958-124">This example follows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe958-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe958-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="c"></a>[<span data-ttu-id="fe958-126">C#</span><span class="sxs-lookup"><span data-stu-id="fe958-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe958-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe958-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe958-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe958-128">Objective-C</span></span>](#tab/objc)
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


