---
author: JeremyKelley
description: Отмена доступа к ресурсу DriveItem.
ms.date: 09/10/2017
title: Отмена доступа к элементу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6cbce9310f8538687f7acbc04ebbd8e2c4000b89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992432"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="97862-103">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="97862-103">Delete a sharing permission from a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97862-104">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="97862-104">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="97862-105">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="97862-105">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="97862-106">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="97862-106">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="97862-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97862-107">Permissions</span></span>
<span data-ttu-id="97862-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97862-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97862-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97862-110">Permission type</span></span>      | <span data-ttu-id="97862-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97862-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97862-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97862-112">Delegated (work or school account)</span></span> | <span data-ttu-id="97862-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97862-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="97862-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97862-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97862-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97862-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="97862-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97862-116">Application</span></span> | <span data-ttu-id="97862-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97862-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97862-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97862-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="97862-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97862-119">Optional request headers</span></span>

| <span data-ttu-id="97862-120">Имя</span><span class="sxs-lookup"><span data-stu-id="97862-120">Name</span></span>          | <span data-ttu-id="97862-121">Тип</span><span class="sxs-lookup"><span data-stu-id="97862-121">Type</span></span>   | <span data-ttu-id="97862-122">Описание</span><span class="sxs-lookup"><span data-stu-id="97862-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="97862-123">if-match</span><span class="sxs-lookup"><span data-stu-id="97862-123">if-match</span></span>      | <span data-ttu-id="97862-124">string</span><span class="sxs-lookup"><span data-stu-id="97862-124">string</span></span> | <span data-ttu-id="97862-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="97862-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="97862-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="97862-126">Response</span></span>

<span data-ttu-id="97862-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97862-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97862-128">Пример</span><span class="sxs-lookup"><span data-stu-id="97862-128">Example</span></span>

<span data-ttu-id="97862-129">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="97862-129">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97862-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="97862-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97862-131">C#</span><span class="sxs-lookup"><span data-stu-id="97862-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97862-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="97862-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97862-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="97862-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97862-134">Java</span><span class="sxs-lookup"><span data-stu-id="97862-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97862-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="97862-135">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="97862-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="97862-136">Remarks</span></span>

* <span data-ttu-id="97862-137">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="97862-137">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
  ]
}
-->
