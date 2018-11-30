---
title: Восстановление предыдущей версии ресурса ListItem
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
ms.openlocfilehash: f8dc4196c40c51287e93aaa667c325e8d4f6dcfb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026184"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="33c3f-104">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="33c3f-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="33c3f-105">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="33c3f-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="33c3f-106">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="33c3f-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="33c3f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33c3f-107">Permissions</span></span>

<span data-ttu-id="33c3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="33c3f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33c3f-110">Permission type</span></span>             |         <span data-ttu-id="33c3f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33c3f-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="33c3f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33c3f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="33c3f-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="33c3f-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="33c3f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33c3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33c3f-115">Н/д</span><span class="sxs-lookup"><span data-stu-id="33c3f-115">n/a</span></span>                                                          |
| <span data-ttu-id="33c3f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33c3f-116">Application</span></span>                            | <span data-ttu-id="33c3f-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="33c3f-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33c3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33c3f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="33c3f-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33c3f-119">Request body</span></span>

<span data-ttu-id="33c3f-120">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="33c3f-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="33c3f-121">Пример</span><span class="sxs-lookup"><span data-stu-id="33c3f-121">Example</span></span>

<span data-ttu-id="33c3f-122">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="33c3f-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="33c3f-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="33c3f-123">Response</span></span>

<span data-ttu-id="33c3f-124">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="33c3f-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
