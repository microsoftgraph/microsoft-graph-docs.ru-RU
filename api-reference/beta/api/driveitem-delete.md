---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b9b48cc5fd0ad3c35a8052571096c24699fdff7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589564"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="44c72-102">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="44c72-102">Delete a DriveItem</span></span>

<span data-ttu-id="44c72-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="44c72-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="44c72-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44c72-105">Permissions</span></span>

<span data-ttu-id="44c72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44c72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44c72-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44c72-108">Permission type</span></span>      | <span data-ttu-id="44c72-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44c72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44c72-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44c72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44c72-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c72-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="44c72-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44c72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c72-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c72-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="44c72-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44c72-114">Application</span></span> | <span data-ttu-id="44c72-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c72-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44c72-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44c72-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="44c72-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44c72-117">Optional request headers</span></span>

| <span data-ttu-id="44c72-118">Имя</span><span class="sxs-lookup"><span data-stu-id="44c72-118">Name</span></span>          | <span data-ttu-id="44c72-119">Тип</span><span class="sxs-lookup"><span data-stu-id="44c72-119">Type</span></span>   | <span data-ttu-id="44c72-120">Описание</span><span class="sxs-lookup"><span data-stu-id="44c72-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="44c72-121">if-match</span><span class="sxs-lookup"><span data-stu-id="44c72-121">if-match</span></span>      | <span data-ttu-id="44c72-122">String</span><span class="sxs-lookup"><span data-stu-id="44c72-122">String</span></span> | <span data-ttu-id="44c72-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="44c72-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="44c72-124">Пример</span><span class="sxs-lookup"><span data-stu-id="44c72-124">Example</span></span>

<span data-ttu-id="44c72-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="44c72-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="44c72-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="44c72-126">Response</span></span>

<span data-ttu-id="44c72-127">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="44c72-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="44c72-128">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="44c72-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="44c72-129">Языках</span><span class="sxs-lookup"><span data-stu-id="44c72-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44c72-130">Язык</span><span class="sxs-lookup"><span data-stu-id="44c72-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="44c72-131">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="44c72-131">Error responses</span></span>

<span data-ttu-id="44c72-132">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="44c72-132">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
