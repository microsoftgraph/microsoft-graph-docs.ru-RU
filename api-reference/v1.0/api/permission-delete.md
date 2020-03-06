---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отмена доступа к элементу
localization_priority: Normal
description: Отмена доступа к ресурсу DriveItem.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: edaa9fe046bcde6bd235d3689bb0b0c0a1538c73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511056"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="56d83-103">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="56d83-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="56d83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56d83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56d83-105">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="56d83-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="56d83-106">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="56d83-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="56d83-107">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="56d83-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="56d83-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56d83-108">Permissions</span></span>

<span data-ttu-id="56d83-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d83-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56d83-111">Permission type</span></span>      | <span data-ttu-id="56d83-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56d83-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d83-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56d83-113">Delegated (work or school account)</span></span> | <span data-ttu-id="56d83-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d83-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56d83-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56d83-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d83-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d83-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="56d83-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56d83-117">Application</span></span> | <span data-ttu-id="56d83-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d83-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d83-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56d83-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="56d83-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56d83-120">Optional request headers</span></span>

| <span data-ttu-id="56d83-121">Имя</span><span class="sxs-lookup"><span data-stu-id="56d83-121">Name</span></span>          | <span data-ttu-id="56d83-122">Тип</span><span class="sxs-lookup"><span data-stu-id="56d83-122">Type</span></span>   | <span data-ttu-id="56d83-123">Описание</span><span class="sxs-lookup"><span data-stu-id="56d83-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="56d83-124">if-match</span><span class="sxs-lookup"><span data-stu-id="56d83-124">if-match</span></span>      | <span data-ttu-id="56d83-125">string</span><span class="sxs-lookup"><span data-stu-id="56d83-125">string</span></span> | <span data-ttu-id="56d83-126">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="56d83-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="56d83-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d83-127">Response</span></span>

<span data-ttu-id="56d83-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56d83-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56d83-129">Пример</span><span class="sxs-lookup"><span data-stu-id="56d83-129">Example</span></span>

<span data-ttu-id="56d83-130">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="56d83-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="56d83-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="56d83-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="56d83-132">C#</span><span class="sxs-lookup"><span data-stu-id="56d83-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56d83-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d83-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56d83-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56d83-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56d83-135">Java</span><span class="sxs-lookup"><span data-stu-id="56d83-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56d83-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d83-136">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="56d83-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="56d83-137">Remarks</span></span>

* <span data-ttu-id="56d83-138">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="56d83-138">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions",
  "suppressions": [
  ]
} -->
