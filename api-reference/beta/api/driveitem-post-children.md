---
author: JeremyKelley
description: Создание папки или ресурса DriveItem в объекте Drive с указанным родительским элементом или по указанному пути.
ms.date: 09/10/2017
title: Создание папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bcc83002f7ea2469d2a8a83f55885f160c3f7087
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416655"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="0759c-103">Создание папки на диске</span><span class="sxs-lookup"><span data-stu-id="0759c-103">Create a new folder in a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0759c-104">Создание папки или ресурса [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) с указанным родительским элементом или по указанному пути.</span><span class="sxs-lookup"><span data-stu-id="0759c-104">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="0759c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0759c-105">Permissions</span></span>

<span data-ttu-id="0759c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0759c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0759c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0759c-108">Permission type</span></span>      | <span data-ttu-id="0759c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0759c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0759c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0759c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0759c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0759c-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0759c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0759c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0759c-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0759c-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0759c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0759c-114">Application</span></span> | <span data-ttu-id="0759c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0759c-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0759c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0759c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="0759c-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0759c-117">Request body</span></span>

<span data-ttu-id="0759c-118">Предоставьте в тексте запроса описание создаваемого ресурса [DriveItem](../resources/driveitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0759c-118">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="0759c-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="0759c-119">Response</span></span>

<span data-ttu-id="0759c-120">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0759c-120">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0759c-121">Пример</span><span class="sxs-lookup"><span data-stu-id="0759c-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="0759c-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="0759c-122">Request</span></span>

<span data-ttu-id="0759c-123">Ниже показан пример запроса на создание папки в корневой папке OneDrive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="0759c-123">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="0759c-124">Используемое свойство `@microsoft.graph.conflictBehavior` указывает, что если при создании папки оказалось, что уже существует элемент с таким именем, служба должна выбрать новое имя папки.</span><span class="sxs-lookup"><span data-stu-id="0759c-124">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0759c-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="0759c-125">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0759c-126">C#</span><span class="sxs-lookup"><span data-stu-id="0759c-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0759c-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0759c-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0759c-128">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0759c-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0759c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0759c-129">Response</span></span>

<span data-ttu-id="0759c-130">При успешном выполнении этот метод возвращает заново созданную папку в виде ресурса [DriveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="0759c-130">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="0759c-131">Ответ с ошибкой</span><span class="sxs-lookup"><span data-stu-id="0759c-131">Error response</span></span>

<span data-ttu-id="0759c-132">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ответы с ошибкой][error-response].</span><span class="sxs-lookup"><span data-stu-id="0759c-132">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
}
-->
