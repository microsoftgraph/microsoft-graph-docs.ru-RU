---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание папки
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 68d2f6db9868ac262ed65c21f27f60ed6f3d1230
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482247"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="819a8-102">Создание папки на диске</span><span class="sxs-lookup"><span data-stu-id="819a8-102">Create a new folder in a drive</span></span>

<span data-ttu-id="819a8-103">Создание папки или ресурса [DriveItem](../resources/driveitem.md) в объекте [Drive](../resources/drive.md) с указанным родительским элементом или по указанному пути.</span><span class="sxs-lookup"><span data-stu-id="819a8-103">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="819a8-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="819a8-104">Permissions</span></span>

<span data-ttu-id="819a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="819a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="819a8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="819a8-107">Permission type</span></span>      | <span data-ttu-id="819a8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="819a8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="819a8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="819a8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="819a8-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="819a8-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="819a8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="819a8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="819a8-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="819a8-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="819a8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="819a8-113">Application</span></span> | <span data-ttu-id="819a8-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="819a8-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="819a8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="819a8-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="819a8-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="819a8-116">Request body</span></span>

<span data-ttu-id="819a8-117">Предоставьте в тексте запроса описание создаваемого ресурса [DriveItem](../resources/driveitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="819a8-117">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="819a8-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="819a8-118">Response</span></span>

<span data-ttu-id="819a8-119">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="819a8-119">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="819a8-120">Пример</span><span class="sxs-lookup"><span data-stu-id="819a8-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="819a8-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="819a8-121">Request</span></span>

<span data-ttu-id="819a8-122">Ниже показан пример запроса на создание папки в корневой папке OneDrive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="819a8-122">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="819a8-123">Используемое свойство `@microsoft.graph.conflictBehavior` указывает, что если при создании папки оказалось, что уже существует элемент с таким именем, служба должна выбрать новое имя папки.</span><span class="sxs-lookup"><span data-stu-id="819a8-123">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>

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

### <a name="response"></a><span data-ttu-id="819a8-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="819a8-124">Response</span></span>

<span data-ttu-id="819a8-125">При успешном выполнении этот метод возвращает заново созданную папку в виде ресурса [DriveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="819a8-125">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="819a8-126">Ответ с ошибкой</span><span class="sxs-lookup"><span data-stu-id="819a8-126">Error response</span></span>

<span data-ttu-id="819a8-127">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ответы с ошибкой][error-response].</span><span class="sxs-lookup"><span data-stu-id="819a8-127">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder"
} -->
