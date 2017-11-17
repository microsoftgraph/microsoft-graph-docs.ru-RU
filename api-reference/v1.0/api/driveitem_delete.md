---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Удаление файла или папки"
ms.openlocfilehash: 403eba1fbf01df0a5d7c410f2f790e222828b371
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="4459d-102">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="4459d-102">Delete a DriveItem</span></span>

<span data-ttu-id="4459d-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="4459d-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="4459d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4459d-105">Permissions</span></span>

<span data-ttu-id="4459d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4459d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4459d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4459d-108">Permission type</span></span>      | <span data-ttu-id="4459d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4459d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4459d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4459d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4459d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4459d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4459d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4459d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4459d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4459d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4459d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4459d-114">Application</span></span> | <span data-ttu-id="4459d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4459d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4459d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4459d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4459d-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4459d-117">Optional request headers</span></span>

| <span data-ttu-id="4459d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4459d-118">Name</span></span>          | <span data-ttu-id="4459d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4459d-119">Type</span></span>   | <span data-ttu-id="4459d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4459d-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4459d-121">if-match</span><span class="sxs-lookup"><span data-stu-id="4459d-121">if-match</span></span>      | <span data-ttu-id="4459d-122">String</span><span class="sxs-lookup"><span data-stu-id="4459d-122">String</span></span> | <span data-ttu-id="4459d-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="4459d-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="4459d-124">Пример</span><span class="sxs-lookup"><span data-stu-id="4459d-124">Example</span></span>

<span data-ttu-id="4459d-125">Ниже приведен пример, в котором показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="4459d-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="4459d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4459d-126">Response</span></span>

<span data-ttu-id="4459d-127">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="4459d-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="4459d-128">Ошибки</span><span class="sxs-lookup"><span data-stu-id="4459d-128">Error responses</span></span>

<span data-ttu-id="4459d-129">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="4459d-129">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
