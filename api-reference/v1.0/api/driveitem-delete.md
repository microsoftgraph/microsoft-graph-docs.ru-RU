---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
description: Удаление ресурса DriveItem по идентификатору или пути.
doc_type: apiPageType
ms.openlocfilehash: e385c005565819999c3d77066ad636adda92b3d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517771"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="d0628-103">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="d0628-103">Delete a DriveItem</span></span>

<span data-ttu-id="d0628-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0628-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0628-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="d0628-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0628-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0628-107">Permissions</span></span>

<span data-ttu-id="d0628-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0628-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0628-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0628-110">Permission type</span></span>      | <span data-ttu-id="d0628-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0628-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0628-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0628-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0628-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0628-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0628-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0628-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0628-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0628-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0628-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0628-116">Application</span></span> | <span data-ttu-id="d0628-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0628-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0628-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0628-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="d0628-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0628-119">Optional request headers</span></span>

| <span data-ttu-id="d0628-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d0628-120">Name</span></span>          | <span data-ttu-id="d0628-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d0628-121">Type</span></span>   | <span data-ttu-id="d0628-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d0628-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d0628-123">if-match</span><span class="sxs-lookup"><span data-stu-id="d0628-123">if-match</span></span>      | <span data-ttu-id="d0628-124">String</span><span class="sxs-lookup"><span data-stu-id="d0628-124">String</span></span> | <span data-ttu-id="d0628-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="d0628-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="d0628-126">Пример</span><span class="sxs-lookup"><span data-stu-id="d0628-126">Example</span></span>

<span data-ttu-id="d0628-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d0628-127">Here is an example of how to call this API.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0628-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0628-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="d0628-129">C#</span><span class="sxs-lookup"><span data-stu-id="d0628-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0628-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0628-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0628-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0628-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0628-132">Java</span><span class="sxs-lookup"><span data-stu-id="d0628-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d0628-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0628-133">Response</span></span>

<span data-ttu-id="d0628-134">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="d0628-134">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="d0628-135">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="d0628-135">Error responses</span></span>

<span data-ttu-id="d0628-136">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="d0628-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
} -->
