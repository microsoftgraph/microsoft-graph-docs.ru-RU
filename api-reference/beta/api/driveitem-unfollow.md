---
author: chackman
ms.author: chackman
title: Отписаться от элемента Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9d43121f4db421bb934e2cce0f045386138b36af
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260020"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="45dd2-102">Отписаться от элемента Drive</span><span class="sxs-lookup"><span data-stu-id="45dd2-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45dd2-103">Отменяйте подписку на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="45dd2-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="45dd2-104">**Примечание:** Чтобы подписаться на элемент, обратитесь к разделу [Отслеживание элемента](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="45dd2-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45dd2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45dd2-105">Permissions</span></span>

<span data-ttu-id="45dd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45dd2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45dd2-108">Permission type</span></span>      | <span data-ttu-id="45dd2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45dd2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45dd2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45dd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45dd2-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45dd2-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="45dd2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45dd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45dd2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45dd2-113">Not supported.</span></span>    |
|<span data-ttu-id="45dd2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45dd2-114">Application</span></span> | <span data-ttu-id="45dd2-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45dd2-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45dd2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45dd2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="45dd2-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45dd2-117">Request body</span></span>

<span data-ttu-id="45dd2-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="45dd2-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="45dd2-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="45dd2-119">Response</span></span>

<span data-ttu-id="45dd2-120">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45dd2-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="45dd2-121">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="45dd2-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45dd2-122">Пример</span><span class="sxs-lookup"><span data-stu-id="45dd2-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="45dd2-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="45dd2-123">Request</span></span>
<span data-ttu-id="45dd2-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45dd2-124">Here is an example of the request.</span></span>
<span data-ttu-id="45dd2-125">В этом примере отменяется отслеживание элемента, `{item-id}`указанного в параметре.</span><span class="sxs-lookup"><span data-stu-id="45dd2-125">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a><span data-ttu-id="45dd2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="45dd2-126">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="45dd2-127">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="45dd2-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="45dd2-128">C#</span><span class="sxs-lookup"><span data-stu-id="45dd2-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/unfollow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45dd2-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="45dd2-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/unfollow-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="45dd2-130">Цель — C</span><span class="sxs-lookup"><span data-stu-id="45dd2-130">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/unfollow-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
