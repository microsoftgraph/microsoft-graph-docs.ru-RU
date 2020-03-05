---
author: JeremyKelley
description: Отмена доступа к ресурсу DriveItem.
ms.date: 09/10/2017
title: Отмена доступа к элементу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a7990bf666dd18bfc0e04d5874fe176ed48e909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455979"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="05480-103">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="05480-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="05480-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="05480-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05480-105">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="05480-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="05480-106">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="05480-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="05480-107">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="05480-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="05480-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05480-108">Permissions</span></span>
<span data-ttu-id="05480-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05480-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05480-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05480-111">Permission type</span></span>      | <span data-ttu-id="05480-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05480-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05480-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05480-113">Delegated (work or school account)</span></span> | <span data-ttu-id="05480-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05480-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="05480-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05480-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05480-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05480-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="05480-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05480-117">Application</span></span> | <span data-ttu-id="05480-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05480-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05480-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05480-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="05480-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05480-120">Optional request headers</span></span>

| <span data-ttu-id="05480-121">Имя</span><span class="sxs-lookup"><span data-stu-id="05480-121">Name</span></span>          | <span data-ttu-id="05480-122">Тип</span><span class="sxs-lookup"><span data-stu-id="05480-122">Type</span></span>   | <span data-ttu-id="05480-123">Описание</span><span class="sxs-lookup"><span data-stu-id="05480-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="05480-124">if-match</span><span class="sxs-lookup"><span data-stu-id="05480-124">if-match</span></span>      | <span data-ttu-id="05480-125">string</span><span class="sxs-lookup"><span data-stu-id="05480-125">string</span></span> | <span data-ttu-id="05480-126">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="05480-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="05480-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="05480-127">Response</span></span>

<span data-ttu-id="05480-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="05480-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05480-129">Пример</span><span class="sxs-lookup"><span data-stu-id="05480-129">Example</span></span>

<span data-ttu-id="05480-130">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="05480-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="05480-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="05480-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="05480-132">C#</span><span class="sxs-lookup"><span data-stu-id="05480-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05480-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05480-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05480-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05480-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05480-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="05480-135">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="05480-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="05480-136">Remarks</span></span>

* <span data-ttu-id="05480-137">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="05480-137">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

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
