---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Перемещение файла или папки
localization_priority: Normal
ms.prod: sharepoint
description: Чтобы переместить ресурс DriveItem в новый родительский элемент, веб-приложению требуется обновить элемент parentReference из DriveItem.
doc_type: apiPageType
ms.openlocfilehash: e94b218c0c67f077a02c8112054db2f2862cc3ab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373448"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="6a8cc-103">Перемещение ресурса DriveItem в новую папку</span><span class="sxs-lookup"><span data-stu-id="6a8cc-103">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="6a8cc-104">Чтобы переместить ресурс DriveItem в новый родительский элемент, вашему приложению требуется обновить элемент **parentReference** ресурса DriveItem, который необходимо переместить.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-104">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="6a8cc-105">Это особый случай, касающийся метода [Обновление](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="6a8cc-105">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="6a8cc-106">Приложение может объединять процедуры перемещения элемента в новый контейнер и обновления других свойств элемента в один запрос.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-106">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="6a8cc-107">С помощью этого запроса не удастся переместить элементы между объектами [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="6a8cc-107">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a8cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a8cc-108">Permissions</span></span>
<span data-ttu-id="6a8cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a8cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a8cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a8cc-111">Permission type</span></span>      | <span data-ttu-id="6a8cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a8cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a8cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a8cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6a8cc-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8cc-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a8cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a8cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8cc-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8cc-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a8cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a8cc-117">Application</span></span> | <span data-ttu-id="6a8cc-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8cc-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a8cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a8cc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6a8cc-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a8cc-120">Optional request headers</span></span>

| <span data-ttu-id="6a8cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6a8cc-121">Name</span></span>          | <span data-ttu-id="6a8cc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6a8cc-122">Type</span></span>   | <span data-ttu-id="6a8cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6a8cc-123">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6a8cc-124">if-match</span><span class="sxs-lookup"><span data-stu-id="6a8cc-124">if-match</span></span>      | <span data-ttu-id="6a8cc-125">String</span><span class="sxs-lookup"><span data-stu-id="6a8cc-125">String</span></span> | <span data-ttu-id="6a8cc-126">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-126">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a8cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a8cc-127">Request body</span></span>

<span data-ttu-id="6a8cc-p103">В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="6a8cc-131">**Примечание.** При перемещении элементов в корневую папку объекта drive вашему приложению не удастся использовать синтаксис `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-131">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="6a8cc-132">Приложению потребуется предоставить фактический идентификатор корневой папки для ссылки на родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-132">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="6a8cc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a8cc-133">Response</span></span>

<span data-ttu-id="6a8cc-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-134">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a8cc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="6a8cc-135">Example</span></span>

<span data-ttu-id="6a8cc-136">В этом примере показано, как переместить элемент, указанный с помощью идентификатора {item-id}, в папку с идентификатором `new-parent-folder-id` для объекта drive пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-136">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6a8cc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a8cc-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "{new-parent-folder-id}"
  },
  "name": "new-item-name.txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a8cc-138">C#</span><span class="sxs-lookup"><span data-stu-id="6a8cc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a8cc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a8cc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a8cc-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6a8cc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a8cc-141">Java</span><span class="sxs-lookup"><span data-stu-id="6a8cc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a8cc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a8cc-142">Response</span></span>

<span data-ttu-id="6a8cc-143">В примере ниже показан отклик для этого запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="6a8cc-143">The following example shows the response for this move request.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a><span data-ttu-id="6a8cc-144">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="6a8cc-144">Error responses</span></span>

<span data-ttu-id="6a8cc-145">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="6a8cc-145">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
  ]
} -->
