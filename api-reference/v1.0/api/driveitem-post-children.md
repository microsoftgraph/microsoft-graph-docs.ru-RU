---
author: JeremyKelley
ms.date: 09/10/2017
title: Создание папки
localization_priority: Priority
ms.prod: sharepoint
description: Создание папки или ресурса DriveItem в объекте Drive с указанным родительским элементом или по указанному пути.
doc_type: apiPageType
ms.openlocfilehash: 8beb1d210b40258b63d54e7af0fac3ff29b8e8e7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240236"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="642ea-103">Создание папки на диске</span><span class="sxs-lookup"><span data-stu-id="642ea-103">Create a new folder in a drive</span></span>

<span data-ttu-id="642ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="642ea-105">Создание папки или ресурса [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) с указанным родительским элементом или по указанному пути.</span><span class="sxs-lookup"><span data-stu-id="642ea-105">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="642ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="642ea-106">Permissions</span></span>

<span data-ttu-id="642ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="642ea-109">Permission type</span></span>      | <span data-ttu-id="642ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="642ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="642ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="642ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="642ea-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642ea-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="642ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="642ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642ea-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642ea-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="642ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="642ea-115">Application</span></span> | <span data-ttu-id="642ea-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="642ea-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="642ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="642ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="642ea-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="642ea-118">Request body</span></span>

<span data-ttu-id="642ea-119">Предоставьте в тексте запроса описание создаваемого ресурса [DriveItem](../resources/driveitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="642ea-119">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="642ea-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="642ea-120">Response</span></span>

<span data-ttu-id="642ea-121">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="642ea-121">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642ea-122">Пример</span><span class="sxs-lookup"><span data-stu-id="642ea-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="642ea-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="642ea-123">Request</span></span>

<span data-ttu-id="642ea-124">Ниже показан пример запроса на создание папки в корневой папке OneDrive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="642ea-124">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="642ea-125">Используемое свойство `@microsoft.graph.conflictBehavior` указывает, что если при создании папки оказалось, что уже существует элемент с таким именем, служба должна выбрать новое имя папки.</span><span class="sxs-lookup"><span data-stu-id="642ea-125">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="http"></a>[<span data-ttu-id="642ea-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="642ea-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-folder", "scopes": "files.readwrite" } -->

```http
POST /me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { },
  "@microsoft.graph.conflictBehavior": "rename"
}
```
# <a name="c"></a>[<span data-ttu-id="642ea-127">C#</span><span class="sxs-lookup"><span data-stu-id="642ea-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642ea-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642ea-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642ea-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642ea-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642ea-130">Java</span><span class="sxs-lookup"><span data-stu-id="642ea-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="642ea-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="642ea-131">Response</span></span>

<span data-ttu-id="642ea-132">При успешном выполнении этот метод возвращает созданную папку в виде ресурса [DriveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="642ea-132">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "2016-09-20T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "2016-09-20T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

## <a name="error-response"></a><span data-ttu-id="642ea-133">Отклик с ошибкой</span><span class="sxs-lookup"><span data-stu-id="642ea-133">Error response</span></span>

<span data-ttu-id="642ea-134">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="642ea-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
} -->

