---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d4b3222e25d715b64ead1a91c1d3b21e033b2ca6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861264"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="dec9f-102">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="dec9f-102">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dec9f-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="dec9f-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="dec9f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dec9f-105">Permissions</span></span>

<span data-ttu-id="dec9f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dec9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dec9f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dec9f-108">Permission type</span></span>      | <span data-ttu-id="dec9f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dec9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dec9f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dec9f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dec9f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec9f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dec9f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dec9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dec9f-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec9f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dec9f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dec9f-114">Application</span></span> | <span data-ttu-id="dec9f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dec9f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dec9f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dec9f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="dec9f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dec9f-117">Optional request headers</span></span>

| <span data-ttu-id="dec9f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dec9f-118">Name</span></span>          | <span data-ttu-id="dec9f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dec9f-119">Type</span></span>   | <span data-ttu-id="dec9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dec9f-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dec9f-121">if-match</span><span class="sxs-lookup"><span data-stu-id="dec9f-121">if-match</span></span>      | <span data-ttu-id="dec9f-122">String</span><span class="sxs-lookup"><span data-stu-id="dec9f-122">String</span></span> | <span data-ttu-id="dec9f-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="dec9f-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="dec9f-124">Пример</span><span class="sxs-lookup"><span data-stu-id="dec9f-124">Example</span></span>

<span data-ttu-id="dec9f-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dec9f-125">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dec9f-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="dec9f-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dec9f-127">C#</span><span class="sxs-lookup"><span data-stu-id="dec9f-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dec9f-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="dec9f-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dec9f-129">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dec9f-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dec9f-130">Java</span><span class="sxs-lookup"><span data-stu-id="dec9f-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dec9f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="dec9f-131">Response</span></span>

<span data-ttu-id="dec9f-132">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="dec9f-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="dec9f-133">Ошибки</span><span class="sxs-lookup"><span data-stu-id="dec9f-133">Error responses</span></span>

<span data-ttu-id="dec9f-134">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="dec9f-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
