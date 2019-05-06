---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aaee21e48cba0a317600e2d1a5ab3fc29e9c02c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589263"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="ef5ea-102">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="ef5ea-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef5ea-103">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="ef5ea-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef5ea-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef5ea-104">Permissions</span></span>

<span data-ttu-id="ef5ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef5ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef5ea-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef5ea-107">Permission type</span></span>      | <span data-ttu-id="ef5ea-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef5ea-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef5ea-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef5ea-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ef5ea-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef5ea-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef5ea-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef5ea-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef5ea-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef5ea-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef5ea-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef5ea-113">Application</span></span> | <span data-ttu-id="ef5ea-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef5ea-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef5ea-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef5ea-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="ef5ea-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef5ea-116">Request body</span></span>

<span data-ttu-id="ef5ea-117">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="ef5ea-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="ef5ea-118">Пример</span><span class="sxs-lookup"><span data-stu-id="ef5ea-118">Example</span></span>

<span data-ttu-id="ef5ea-119">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="ef5ea-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="ef5ea-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef5ea-120">Response</span></span>

<span data-ttu-id="ef5ea-121">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="ef5ea-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ef5ea-122">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ef5ea-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ef5ea-123">Языках</span><span class="sxs-lookup"><span data-stu-id="ef5ea-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/checkout-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef5ea-124">Язык</span><span class="sxs-lookup"><span data-stu-id="ef5ea-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/checkout-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="remarks"></a><span data-ttu-id="ef5ea-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef5ea-125">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
