---
author: JeremyKelley
description: Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет записан после изменения.
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: eeaa36c2aa71469572a31f02b5692727508a62fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957229"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="2346b-103">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="2346b-103">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2346b-104">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="2346b-104">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2346b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2346b-105">Permissions</span></span>

<span data-ttu-id="2346b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2346b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2346b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2346b-108">Permission type</span></span>      | <span data-ttu-id="2346b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2346b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2346b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2346b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2346b-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2346b-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2346b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2346b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2346b-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2346b-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2346b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2346b-114">Application</span></span> | <span data-ttu-id="2346b-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2346b-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2346b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2346b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="2346b-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2346b-117">Request body</span></span>

<span data-ttu-id="2346b-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="2346b-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="2346b-119">Пример</span><span class="sxs-lookup"><span data-stu-id="2346b-119">Example</span></span>

<span data-ttu-id="2346b-120">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="2346b-120">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2346b-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="2346b-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2346b-122">C#</span><span class="sxs-lookup"><span data-stu-id="2346b-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2346b-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="2346b-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2346b-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2346b-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2346b-125">Java</span><span class="sxs-lookup"><span data-stu-id="2346b-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="2346b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2346b-126">Response</span></span>

<span data-ttu-id="2346b-127">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="2346b-127">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="2346b-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="2346b-128">Remarks</span></span>


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
