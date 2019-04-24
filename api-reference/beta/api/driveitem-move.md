---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Перемещение файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 18bd8493babed354576c5b8066b3bab5de537e65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454339"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="6e79c-102">Перемещение ресурса DriveItem в новую папку</span><span class="sxs-lookup"><span data-stu-id="6e79c-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="6e79c-103">Чтобы переместить ресурс DriveItem в новый родительский элемент, вашему приложению требуется обновить элемент **parentReference** ресурса DriveItem, который необходимо переместить.</span><span class="sxs-lookup"><span data-stu-id="6e79c-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="6e79c-104">Это особый случай, касающийся метода [Обновление](driveitem-update.md).</span><span class="sxs-lookup"><span data-stu-id="6e79c-104">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="6e79c-105">Приложение может объединять процедуры перемещения элемента в новый контейнер и обновления других свойств элемента в один запрос.</span><span class="sxs-lookup"><span data-stu-id="6e79c-105">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="6e79c-106">С помощью этого запроса не удастся переместить элементы между объектами [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="6e79c-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e79c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e79c-107">Permissions</span></span>
<span data-ttu-id="6e79c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e79c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e79c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e79c-110">Permission type</span></span>      | <span data-ttu-id="6e79c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e79c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e79c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e79c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e79c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e79c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e79c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e79c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e79c-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e79c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e79c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e79c-116">Application</span></span> | <span data-ttu-id="6e79c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e79c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e79c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e79c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6e79c-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e79c-119">Optional request headers</span></span>

| <span data-ttu-id="6e79c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6e79c-120">Name</span></span>          | <span data-ttu-id="6e79c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6e79c-121">Type</span></span>   | <span data-ttu-id="6e79c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6e79c-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6e79c-123">if-match</span><span class="sxs-lookup"><span data-stu-id="6e79c-123">if-match</span></span>      | <span data-ttu-id="6e79c-124">String</span><span class="sxs-lookup"><span data-stu-id="6e79c-124">String</span></span> | <span data-ttu-id="6e79c-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="6e79c-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e79c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e79c-126">Request body</span></span>

<span data-ttu-id="6e79c-p103">В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6e79c-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="6e79c-130">**Примечание.** При перемещении элементов в корневую папку объекта drive вашему приложению не удастся использовать синтаксис `"id:" "root"`.</span><span class="sxs-lookup"><span data-stu-id="6e79c-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="6e79c-131">Приложению потребуется предоставить фактический идентификатор корневой папки для ссылки на родительский элемент.</span><span class="sxs-lookup"><span data-stu-id="6e79c-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="6e79c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e79c-132">Response</span></span>

<span data-ttu-id="6e79c-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e79c-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e79c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6e79c-134">Example</span></span>

<span data-ttu-id="6e79c-135">В этом примере показано, как переместить элемент, указанный с помощью идентификатора {item-id}, в папку с идентификатором `new-parent-folder-id` для объекта drive пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e79c-135">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>

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

### <a name="response"></a><span data-ttu-id="6e79c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e79c-136">Response</span></span>

<span data-ttu-id="6e79c-137">В примере ниже показан отклик для этого запроса на перемещение.</span><span class="sxs-lookup"><span data-stu-id="6e79c-137">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="6e79c-138">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="6e79c-138">Error responses</span></span>

<span data-ttu-id="6e79c-139">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="6e79c-139">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
