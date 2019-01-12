---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Удаление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 40b29bee213da3693917a37b14368112ea295c12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926241"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="2314f-102">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="2314f-102">Delete a DriveItem</span></span>

> <span data-ttu-id="2314f-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2314f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2314f-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2314f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2314f-p102">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="2314f-p102">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="2314f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2314f-107">Permissions</span></span>

<span data-ttu-id="2314f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2314f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2314f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2314f-110">Permission type</span></span>      | <span data-ttu-id="2314f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2314f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2314f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2314f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2314f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2314f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2314f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2314f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2314f-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2314f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2314f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2314f-116">Application</span></span> | <span data-ttu-id="2314f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2314f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2314f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2314f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="2314f-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2314f-119">Optional request headers</span></span>

| <span data-ttu-id="2314f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2314f-120">Name</span></span>          | <span data-ttu-id="2314f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2314f-121">Type</span></span>   | <span data-ttu-id="2314f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2314f-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2314f-123">if-match</span><span class="sxs-lookup"><span data-stu-id="2314f-123">if-match</span></span>      | <span data-ttu-id="2314f-124">String</span><span class="sxs-lookup"><span data-stu-id="2314f-124">String</span></span> | <span data-ttu-id="2314f-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="2314f-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="2314f-126">Пример</span><span class="sxs-lookup"><span data-stu-id="2314f-126">Example</span></span>

<span data-ttu-id="2314f-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2314f-127">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="2314f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2314f-128">Response</span></span>

<span data-ttu-id="2314f-129">При успешном выполнении этот запрос возвращает ответ `204 No Content`, указывающий, что ресурс был удален и что нет данных, которые необходимо возвратить.</span><span class="sxs-lookup"><span data-stu-id="2314f-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="2314f-130">Ошибки</span><span class="sxs-lookup"><span data-stu-id="2314f-130">Error responses</span></span>

<span data-ttu-id="2314f-131">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="2314f-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
