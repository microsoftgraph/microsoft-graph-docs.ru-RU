---
author: JeremyKelley
description: Извлеките ресурс driveItem, чтобы другие пользователи не могли редактировать документ, а ваши изменения будут видны, пока они не будут возвращены.
title: 'driveItem: Checkout'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 69f01b949d38d76be24834151c10581589b75e2e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43227591"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="f0797-103">driveItem: Checkout</span><span class="sxs-lookup"><span data-stu-id="f0797-103">driveItem: checkout</span></span>

<span data-ttu-id="f0797-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0797-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0797-105">Извлеките ресурс **driveItem** , чтобы другие пользователи не могли редактировать документ, и не допускают изменения, пока не будет [возвращено](driveitem-checkin.md)задокументированное значение.</span><span class="sxs-lookup"><span data-stu-id="f0797-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0797-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0797-106">Permissions</span></span>

<span data-ttu-id="f0797-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0797-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0797-109">Permission type</span></span>      | <span data-ttu-id="f0797-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0797-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0797-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0797-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0797-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0797-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0797-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0797-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0797-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0797-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0797-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0797-115">Application</span></span> | <span data-ttu-id="f0797-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0797-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0797-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0797-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="f0797-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0797-118">Request body</span></span>

<span data-ttu-id="f0797-119">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="f0797-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f0797-120">Пример</span><span class="sxs-lookup"><span data-stu-id="f0797-120">Example</span></span>

<span data-ttu-id="f0797-121">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="f0797-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0797-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0797-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="f0797-123">C#</span><span class="sxs-lookup"><span data-stu-id="f0797-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0797-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0797-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0797-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0797-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f0797-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0797-126">Response</span></span>

<span data-ttu-id="f0797-127">В случае успеха вызов API возвращает `204 No content` .</span><span class="sxs-lookup"><span data-stu-id="f0797-127">If successful, the API call returns `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="f0797-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="f0797-128">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
