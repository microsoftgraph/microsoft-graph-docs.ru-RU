---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Отмена доступа к элементу
ms.openlocfilehash: a9f98bd7d05f56044aa4193a9ef8e3f565ab22aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027239"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="4b715-102">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="4b715-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="4b715-103">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4b715-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="4b715-104">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="4b715-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="4b715-105">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="4b715-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b715-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b715-106">Permissions</span></span>

<span data-ttu-id="4b715-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b715-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b715-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b715-109">Permission type</span></span>      | <span data-ttu-id="4b715-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b715-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b715-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b715-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b715-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b715-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b715-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b715-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b715-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b715-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b715-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b715-115">Application</span></span> | <span data-ttu-id="4b715-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b715-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b715-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b715-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4b715-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b715-118">Optional request headers</span></span>

| <span data-ttu-id="4b715-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4b715-119">Name</span></span>          | <span data-ttu-id="4b715-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4b715-120">Type</span></span>   | <span data-ttu-id="4b715-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4b715-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b715-122">if-match</span><span class="sxs-lookup"><span data-stu-id="4b715-122">if-match</span></span>      | <span data-ttu-id="4b715-123">string</span><span class="sxs-lookup"><span data-stu-id="4b715-123">string</span></span> | <span data-ttu-id="4b715-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="4b715-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="4b715-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b715-125">Response</span></span>

<span data-ttu-id="4b715-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4b715-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b715-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4b715-127">Example</span></span>

<span data-ttu-id="4b715-128">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b715-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="4b715-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b715-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="4b715-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="4b715-130">Remarks</span></span>

* <span data-ttu-id="4b715-131">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4b715-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions"
} -->
