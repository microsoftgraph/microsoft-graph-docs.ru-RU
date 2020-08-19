---
title: Восстановление предыдущей версии ресурса ListItem
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: f8f7aa23a1db378dea805ed5250c0d27e3d0c554
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812704"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="1794d-104">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="1794d-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="1794d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1794d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1794d-106">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="1794d-106">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="1794d-107">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="1794d-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="1794d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1794d-108">Permissions</span></span>

<span data-ttu-id="1794d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1794d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1794d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1794d-111">Permission type</span></span>             |         <span data-ttu-id="1794d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1794d-112">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1794d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1794d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1794d-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1794d-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="1794d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1794d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1794d-116">Н/д</span><span class="sxs-lookup"><span data-stu-id="1794d-116">n/a</span></span>                                                          |
| <span data-ttu-id="1794d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1794d-117">Application</span></span>                            | <span data-ttu-id="1794d-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1794d-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1794d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1794d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="1794d-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1794d-120">Request body</span></span>

<span data-ttu-id="1794d-121">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="1794d-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="1794d-122">Пример</span><span class="sxs-lookup"><span data-stu-id="1794d-122">Example</span></span>

<span data-ttu-id="1794d-123">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="1794d-123">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="1794d-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="1794d-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="1794d-125">C#</span><span class="sxs-lookup"><span data-stu-id="1794d-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1794d-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1794d-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1794d-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1794d-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1794d-128">Java</span><span class="sxs-lookup"><span data-stu-id="1794d-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="1794d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1794d-129">Response</span></span>

<span data-ttu-id="1794d-130">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1794d-130">If successful, the API call returns a `204 No Content`.</span></span>

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
