---
author: JeremyKelley
description: Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет записан после изменения.
ms.date: 09/10/2017
title: Извлечение файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4159882b29dc69429a7b99bb89d1e8051d6e9c03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432945"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="d71f0-103">Получение ресурса DriveItem для изменения</span><span class="sxs-lookup"><span data-stu-id="d71f0-103">Check-out a DriveItem resource</span></span>

<span data-ttu-id="d71f0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d71f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d71f0-105">Вы можете получить ресурс driveItem для изменения, чтобы другие пользователи не могли редактировать документ, а внесенные вами изменения не отображались, пока документ не будет [записан после изменения](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="d71f0-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d71f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d71f0-106">Permissions</span></span>

<span data-ttu-id="d71f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d71f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d71f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d71f0-109">Permission type</span></span>      | <span data-ttu-id="d71f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d71f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d71f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d71f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d71f0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d71f0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d71f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d71f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d71f0-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d71f0-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d71f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d71f0-115">Application</span></span> | <span data-ttu-id="d71f0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d71f0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d71f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d71f0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="d71f0-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d71f0-118">Request body</span></span>

<span data-ttu-id="d71f0-119">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="d71f0-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="d71f0-120">Пример</span><span class="sxs-lookup"><span data-stu-id="d71f0-120">Example</span></span>

<span data-ttu-id="d71f0-121">В этом примере показано, как записать после изменения файл, указанный по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="d71f0-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="d71f0-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="d71f0-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="d71f0-123">C#</span><span class="sxs-lookup"><span data-stu-id="d71f0-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d71f0-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d71f0-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d71f0-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d71f0-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d71f0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d71f0-126">Response</span></span>

<span data-ttu-id="d71f0-127">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="d71f0-127">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="d71f0-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="d71f0-128">Remarks</span></span>


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
