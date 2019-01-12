---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 39c7706fab229e52c394c30c6daf478a1fefd581
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966869"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="ac5b0-102">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="ac5b0-102">Delete a DriveItem</span></span>

<span data-ttu-id="ac5b0-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="ac5b0-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac5b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5b0-105">Permissions</span></span>

<span data-ttu-id="ac5b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac5b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac5b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5b0-108">Permission type</span></span>      | <span data-ttu-id="ac5b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac5b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac5b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac5b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac5b0-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5b0-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac5b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac5b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac5b0-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5b0-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac5b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac5b0-114">Application</span></span> | <span data-ttu-id="ac5b0-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5b0-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac5b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac5b0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ac5b0-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac5b0-117">Optional request headers</span></span>

| <span data-ttu-id="ac5b0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ac5b0-118">Name</span></span>          | <span data-ttu-id="ac5b0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ac5b0-119">Type</span></span>   | <span data-ttu-id="ac5b0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5b0-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ac5b0-121">if-match</span><span class="sxs-lookup"><span data-stu-id="ac5b0-121">if-match</span></span>      | <span data-ttu-id="ac5b0-122">String</span><span class="sxs-lookup"><span data-stu-id="ac5b0-122">String</span></span> | <span data-ttu-id="ac5b0-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="ac5b0-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="ac5b0-124">Пример</span><span class="sxs-lookup"><span data-stu-id="ac5b0-124">Example</span></span>

<span data-ttu-id="ac5b0-125">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ac5b0-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="ac5b0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac5b0-126">Response</span></span>

<span data-ttu-id="ac5b0-127">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="ac5b0-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="ac5b0-128">Ошибки</span><span class="sxs-lookup"><span data-stu-id="ac5b0-128">Error responses</span></span>

<span data-ttu-id="ac5b0-129">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="ac5b0-129">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
