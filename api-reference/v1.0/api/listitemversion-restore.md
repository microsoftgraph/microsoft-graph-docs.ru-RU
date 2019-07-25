---
title: Восстановление предыдущей версии ресурса ListItem
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8c6c4a67988d9e073942c44b9787cfa91330dbeb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885830"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="fce85-104">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="fce85-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="fce85-105">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="fce85-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="fce85-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="fce85-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="fce85-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fce85-107">Permissions</span></span>

<span data-ttu-id="fce85-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce85-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="fce85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fce85-110">Permission type</span></span>             |         <span data-ttu-id="fce85-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fce85-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="fce85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fce85-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fce85-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fce85-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="fce85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fce85-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fce85-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="fce85-115">n/a</span></span>                                                          |
| <span data-ttu-id="fce85-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fce85-116">Application</span></span>                            | <span data-ttu-id="fce85-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="fce85-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fce85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fce85-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="fce85-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fce85-119">Request body</span></span>

<span data-ttu-id="fce85-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="fce85-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="fce85-121">Пример</span><span class="sxs-lookup"><span data-stu-id="fce85-121">Example</span></span>

<span data-ttu-id="fce85-122">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="fce85-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fce85-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="fce85-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fce85-124">C#</span><span class="sxs-lookup"><span data-stu-id="fce85-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fce85-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="fce85-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fce85-126">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fce85-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fce85-127">Java</span><span class="sxs-lookup"><span data-stu-id="fce85-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="fce85-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fce85-128">Response</span></span>

<span data-ttu-id="fce85-129">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fce85-129">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
