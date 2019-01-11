---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Отмена доступа к элементу
localization_priority: Normal
ms.openlocfilehash: 4f22082c8f9ce540d3c1c1188c8f9c5ff06ab525
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810026"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="049a1-102">Удаление разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="049a1-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="049a1-103">В этой статье рассказывается, как отменить доступ к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="049a1-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="049a1-104">Вы можете удалить только те разрешения на общий доступ, которые **не** были унаследованы.</span><span class="sxs-lookup"><span data-stu-id="049a1-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="049a1-105">Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="049a1-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="049a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="049a1-106">Permissions</span></span>

<span data-ttu-id="049a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="049a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="049a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="049a1-109">Permission type</span></span>      | <span data-ttu-id="049a1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="049a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="049a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="049a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="049a1-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049a1-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="049a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="049a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="049a1-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049a1-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="049a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="049a1-115">Application</span></span> | <span data-ttu-id="049a1-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049a1-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="049a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="049a1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="049a1-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="049a1-118">Optional request headers</span></span>

| <span data-ttu-id="049a1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="049a1-119">Name</span></span>          | <span data-ttu-id="049a1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="049a1-120">Type</span></span>   | <span data-ttu-id="049a1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="049a1-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="049a1-122">if-match</span><span class="sxs-lookup"><span data-stu-id="049a1-122">if-match</span></span>      | <span data-ttu-id="049a1-123">string</span><span class="sxs-lookup"><span data-stu-id="049a1-123">string</span></span> | <span data-ttu-id="049a1-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="049a1-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="049a1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="049a1-125">Response</span></span>

<span data-ttu-id="049a1-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="049a1-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="049a1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="049a1-127">Example</span></span>

<span data-ttu-id="049a1-128">В этом примере показано, как удалить разрешение, идентифицированное как {perm-id} из элемента {item-id} в хранилище OneDrive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="049a1-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="049a1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="049a1-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="049a1-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="049a1-130">Remarks</span></span>

* <span data-ttu-id="049a1-131">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="049a1-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions"
} -->
