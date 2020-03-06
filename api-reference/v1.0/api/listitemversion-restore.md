---
title: Восстановление предыдущей версии ресурса ListItem
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: c6109575256ed6a90019b4da1d88723a163569b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511672"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="02507-104">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="02507-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="02507-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02507-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02507-106">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="02507-106">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="02507-107">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="02507-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="02507-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02507-108">Permissions</span></span>

<span data-ttu-id="02507-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02507-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="02507-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02507-111">Permission type</span></span>             |         <span data-ttu-id="02507-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02507-112">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="02507-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02507-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="02507-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="02507-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="02507-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02507-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02507-116">Н/д</span><span class="sxs-lookup"><span data-stu-id="02507-116">n/a</span></span>                                                          |
| <span data-ttu-id="02507-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02507-117">Application</span></span>                            | <span data-ttu-id="02507-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="02507-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02507-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02507-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="02507-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02507-120">Request body</span></span>

<span data-ttu-id="02507-121">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="02507-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="02507-122">Пример</span><span class="sxs-lookup"><span data-stu-id="02507-122">Example</span></span>

<span data-ttu-id="02507-123">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="02507-123">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="02507-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="02507-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="02507-125">C#</span><span class="sxs-lookup"><span data-stu-id="02507-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02507-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02507-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02507-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02507-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02507-128">Java</span><span class="sxs-lookup"><span data-stu-id="02507-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="02507-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="02507-129">Response</span></span>

<span data-ttu-id="02507-130">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02507-130">If successful, the API call returns a `204 No Content`.</span></span>

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
