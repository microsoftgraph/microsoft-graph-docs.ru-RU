---
author: JeremyKelley
description: Удаление ресурса DriveItem по идентификатору или пути.
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7b2df0e8e0cc529238fbc529c0e1281f4c6f258c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957187"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="ba5d0-103">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="ba5d0-103">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba5d0-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="ba5d0-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba5d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5d0-106">Permissions</span></span>

<span data-ttu-id="ba5d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5d0-109">Permission type</span></span>      | <span data-ttu-id="ba5d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba5d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba5d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba5d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba5d0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5d0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba5d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba5d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba5d0-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5d0-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba5d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba5d0-115">Application</span></span> | <span data-ttu-id="ba5d0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5d0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba5d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba5d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ba5d0-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba5d0-118">Optional request headers</span></span>

| <span data-ttu-id="ba5d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba5d0-119">Name</span></span>          | <span data-ttu-id="ba5d0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5d0-120">Type</span></span>   | <span data-ttu-id="ba5d0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5d0-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba5d0-122">if-match</span><span class="sxs-lookup"><span data-stu-id="ba5d0-122">if-match</span></span>      | <span data-ttu-id="ba5d0-123">String</span><span class="sxs-lookup"><span data-stu-id="ba5d0-123">String</span></span> | <span data-ttu-id="ba5d0-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="ba5d0-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="ba5d0-125">Пример</span><span class="sxs-lookup"><span data-stu-id="ba5d0-125">Example</span></span>

<span data-ttu-id="ba5d0-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ba5d0-126">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ba5d0-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba5d0-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba5d0-128">C#</span><span class="sxs-lookup"><span data-stu-id="ba5d0-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba5d0-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba5d0-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba5d0-130">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ba5d0-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ba5d0-131">Java</span><span class="sxs-lookup"><span data-stu-id="ba5d0-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ba5d0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba5d0-132">Response</span></span>

<span data-ttu-id="ba5d0-133">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="ba5d0-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="ba5d0-134">Ошибки</span><span class="sxs-lookup"><span data-stu-id="ba5d0-134">Error responses</span></span>

<span data-ttu-id="ba5d0-135">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="ba5d0-135">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
}
-->
