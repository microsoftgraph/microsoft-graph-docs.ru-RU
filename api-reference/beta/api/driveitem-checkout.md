---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f5447e9e849797081ae96429aaea664abb835a45
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260258"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="52e96-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="52e96-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52e96-103">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="52e96-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="52e96-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52e96-104">Permissions</span></span>

<span data-ttu-id="52e96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e96-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52e96-107">Permission type</span></span>      | <span data-ttu-id="52e96-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52e96-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52e96-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52e96-109">Delegated (work or school account)</span></span> | <span data-ttu-id="52e96-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e96-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="52e96-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52e96-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52e96-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e96-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="52e96-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52e96-113">Application</span></span> | <span data-ttu-id="52e96-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e96-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52e96-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52e96-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="52e96-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52e96-116">Request body</span></span>

<span data-ttu-id="52e96-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="52e96-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="52e96-118">Пример</span><span class="sxs-lookup"><span data-stu-id="52e96-118">Example</span></span>

<span data-ttu-id="52e96-119">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="52e96-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="52e96-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="52e96-120">Response</span></span>

<span data-ttu-id="52e96-121">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="52e96-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52e96-122">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="52e96-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52e96-123">C#</span><span class="sxs-lookup"><span data-stu-id="52e96-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkout-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52e96-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="52e96-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkout-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52e96-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="52e96-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/checkout-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="52e96-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="52e96-126">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
