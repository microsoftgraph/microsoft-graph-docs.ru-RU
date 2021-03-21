---
author: JeremyKelley
description: Отмена доступа к ресурсу DriveItem.
ms.date: 09/10/2017
title: Удаление доступа к элементу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: c581fc01e44a327aeba068295a6583ec040a5042
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962935"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="36417-103">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="36417-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="36417-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36417-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36417-105">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="36417-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="36417-106">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="36417-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="36417-107">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="36417-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="36417-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36417-108">Permissions</span></span>
<span data-ttu-id="36417-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36417-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36417-111">Permission type</span></span>      | <span data-ttu-id="36417-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36417-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36417-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36417-113">Delegated (work or school account)</span></span> | <span data-ttu-id="36417-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36417-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="36417-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36417-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36417-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36417-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="36417-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36417-117">Application</span></span> | <span data-ttu-id="36417-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36417-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36417-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36417-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="36417-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36417-120">Optional request headers</span></span>

| <span data-ttu-id="36417-121">Имя</span><span class="sxs-lookup"><span data-stu-id="36417-121">Name</span></span>          | <span data-ttu-id="36417-122">Тип</span><span class="sxs-lookup"><span data-stu-id="36417-122">Type</span></span>   | <span data-ttu-id="36417-123">Описание</span><span class="sxs-lookup"><span data-stu-id="36417-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="36417-124">if-match</span><span class="sxs-lookup"><span data-stu-id="36417-124">if-match</span></span>      | <span data-ttu-id="36417-125">string</span><span class="sxs-lookup"><span data-stu-id="36417-125">string</span></span> | <span data-ttu-id="36417-126">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="36417-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="36417-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="36417-127">Response</span></span>

<span data-ttu-id="36417-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="36417-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36417-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36417-129">Example</span></span>

<span data-ttu-id="36417-130">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="36417-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>



# <a name="http"></a>[<span data-ttu-id="36417-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="36417-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission-1", "scopes": "files.readwrite" }-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="36417-132">C#</span><span class="sxs-lookup"><span data-stu-id="36417-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36417-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36417-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36417-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36417-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36417-135">Java</span><span class="sxs-lookup"><span data-stu-id="36417-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36417-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="36417-136">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="36417-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="36417-137">Remarks</span></span>

* <span data-ttu-id="36417-138">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="36417-138">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

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


