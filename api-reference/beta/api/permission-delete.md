---
author: JeremyKelley
description: Отмена доступа к ресурсу DriveItem.
ms.date: 09/10/2017
title: Отмена доступа к элементу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 0cc07dba0263516c0d02179ce81d85f9a6fea806
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413729"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="7ef73-103">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="7ef73-103">Delete a sharing permission from a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ef73-104">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7ef73-104">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="7ef73-105">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="7ef73-105">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="7ef73-106">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="7ef73-106">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef73-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef73-107">Permissions</span></span>
<span data-ttu-id="7ef73-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef73-110">Permission type</span></span>      | <span data-ttu-id="7ef73-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ef73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ef73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ef73-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ef73-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef73-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ef73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ef73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ef73-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef73-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ef73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ef73-116">Application</span></span> | <span data-ttu-id="7ef73-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef73-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ef73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef73-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="7ef73-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef73-119">Optional request headers</span></span>

| <span data-ttu-id="7ef73-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7ef73-120">Name</span></span>          | <span data-ttu-id="7ef73-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef73-121">Type</span></span>   | <span data-ttu-id="7ef73-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef73-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7ef73-123">if-match</span><span class="sxs-lookup"><span data-stu-id="7ef73-123">if-match</span></span>      | <span data-ttu-id="7ef73-124">string</span><span class="sxs-lookup"><span data-stu-id="7ef73-124">string</span></span> | <span data-ttu-id="7ef73-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="7ef73-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="7ef73-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef73-126">Response</span></span>

<span data-ttu-id="7ef73-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7ef73-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ef73-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7ef73-128">Example</span></span>

<span data-ttu-id="7ef73-129">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ef73-129">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7ef73-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ef73-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ef73-131">C#</span><span class="sxs-lookup"><span data-stu-id="7ef73-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ef73-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ef73-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ef73-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7ef73-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ef73-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef73-134">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="7ef73-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="7ef73-135">Remarks</span></span>

* <span data-ttu-id="7ef73-136">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="7ef73-136">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

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
