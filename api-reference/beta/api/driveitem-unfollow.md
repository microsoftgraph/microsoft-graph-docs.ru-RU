---
author: chackman
ms.author: chackman
description: Отменяйте подписку на элемент, на который подписан пользователь.
title: Отписаться от элемента Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 29c07176a2d37f7e38deaa4c4020287d82495834
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432329"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="ce8f4-103">Отписаться от элемента Drive</span><span class="sxs-lookup"><span data-stu-id="ce8f4-103">Unfollow drive item</span></span>

<span data-ttu-id="ce8f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce8f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8f4-105">Отменяйте подписку на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ce8f4-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="ce8f4-106">**Примечание:** Чтобы подписаться на элемент, обратитесь к разделу [Отслеживание элемента](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="ce8f4-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce8f4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce8f4-107">Permissions</span></span>

<span data-ttu-id="ce8f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce8f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce8f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce8f4-110">Permission type</span></span>      | <span data-ttu-id="ce8f4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce8f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce8f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce8f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce8f4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8f4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce8f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce8f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce8f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-115">Not supported.</span></span>    |
|<span data-ttu-id="ce8f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce8f4-116">Application</span></span> | <span data-ttu-id="ce8f4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8f4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce8f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce8f4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="ce8f4-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce8f4-119">Request body</span></span>

<span data-ttu-id="ce8f4-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="ce8f4-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce8f4-121">Response</span></span>

<span data-ttu-id="ce8f4-122">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-122">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="ce8f4-123">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-123">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce8f4-124">Пример</span><span class="sxs-lookup"><span data-stu-id="ce8f4-124">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce8f4-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce8f4-125">Request</span></span>
<span data-ttu-id="ce8f4-126">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-126">Here is an example of the request.</span></span>
<span data-ttu-id="ce8f4-127">В этом примере отменяется отслеживание элемента, `{item-id}`указанного в параметре.</span><span class="sxs-lookup"><span data-stu-id="ce8f4-127">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce8f4-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce8f4-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="c"></a>[<span data-ttu-id="ce8f4-129">C#</span><span class="sxs-lookup"><span data-stu-id="ce8f4-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce8f4-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce8f4-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce8f4-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce8f4-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ce8f4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce8f4-132">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->
