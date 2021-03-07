---
author: JeremyKelley
ms.date: 09/10/2017
title: Перемещение файла или папки
localization_priority: Normal
ms.prod: sharepoint
description: Чтобы переместить ресурс DriveItem в новый родительский элемент, веб-приложению требуется обновить элемент parentReference из DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 9465ac1ad39781ee330d134c763c8189e89d208f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516754"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="33093-103">Перемещение ресурса DriveItem в новую папку</span><span class="sxs-lookup"><span data-stu-id="33093-103">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="33093-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33093-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33093-105">Чтобы переместить ресурс DriveItem в новый родительский элемент, веб-приложению требуется обновить элемент **parentReference** из DriveItem.</span><span class="sxs-lookup"><span data-stu-id="33093-105">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="33093-106">Это особый случай, касающийся метода [Обновление](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="33093-106">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="33093-107">Приложение может объединять процедуры перемещения элемента в новый контейнер и обновления других свойств элемента в один запрос.</span><span class="sxs-lookup"><span data-stu-id="33093-107">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="33093-108">С помощью этого запроса не удастся переместить элементы между объектами [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="33093-108">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="33093-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33093-109">Permissions</span></span>
<span data-ttu-id="33093-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33093-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33093-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33093-112">Permission type</span></span>      | <span data-ttu-id="33093-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33093-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33093-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33093-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33093-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33093-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="33093-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33093-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33093-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33093-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="33093-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33093-118">Application</span></span> | <span data-ttu-id="33093-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33093-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33093-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33093-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="33093-121">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33093-121">Optional request headers</span></span>

| <span data-ttu-id="33093-122">Имя</span><span class="sxs-lookup"><span data-stu-id="33093-122">Name</span></span>          | <span data-ttu-id="33093-123">Тип</span><span class="sxs-lookup"><span data-stu-id="33093-123">Type</span></span>   | <span data-ttu-id="33093-124">Описание</span><span class="sxs-lookup"><span data-stu-id="33093-124">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="33093-125">if-match</span><span class="sxs-lookup"><span data-stu-id="33093-125">if-match</span></span>      | <span data-ttu-id="33093-126">String</span><span class="sxs-lookup"><span data-stu-id="33093-126">String</span></span> | <span data-ttu-id="33093-127">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="33093-127">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33093-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33093-128">Request body</span></span>

<span data-ttu-id="33093-p103">В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="33093-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="33093-132">**Примечание.** При перемещении элементов в корневую папку объекта drive вашему приложению не удастся использовать синтаксис `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="33093-132">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="33093-133">Приложению потребуется предоставить фактический идентификатор корневой папки для ссылки на родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="33093-133">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="33093-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="33093-134">Response</span></span>

<span data-ttu-id="33093-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33093-135">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33093-136">Пример</span><span class="sxs-lookup"><span data-stu-id="33093-136">Example</span></span>

<span data-ttu-id="33093-137">В этом примере показано, как переместить элемент, указанный с помощью идентификатора {item-id}, в папку с идентификатором `new-parent-folder-id` для объекта drive пользователя.</span><span class="sxs-lookup"><span data-stu-id="33093-137">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="http"></a>[<span data-ttu-id="33093-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="33093-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33093-139">C#</span><span class="sxs-lookup"><span data-stu-id="33093-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33093-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33093-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33093-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33093-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33093-142">Java</span><span class="sxs-lookup"><span data-stu-id="33093-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="33093-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="33093-143">Response</span></span>

<span data-ttu-id="33093-144">В примере ниже показан отклик для этого запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="33093-144">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="33093-145">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="33093-145">Error responses</span></span>

<span data-ttu-id="33093-146">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="33093-146">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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

