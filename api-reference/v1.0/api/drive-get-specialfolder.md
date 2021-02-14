---
author: JeremyKelley
ms.date: 09/10/2017
title: Получить специальные папки
localization_priority: Normal
ms.prod: sharepoint
description: Используйте специальную коллекцию для доступа к специальной папке по имени.
doc_type: apiPageType
ms.openlocfilehash: bf75cc4355f205fee58ec30291b5f71d7d590df7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239739"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="e6f10-103">Получение доступа к специальной папке по ее имени</span><span class="sxs-lookup"><span data-stu-id="e6f10-103">Get a special folder by name</span></span>

<span data-ttu-id="e6f10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f10-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6f10-105">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="e6f10-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="e6f10-p101">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="e6f10-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="e6f10-p102">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="e6f10-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="e6f10-110">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="e6f10-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f10-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f10-111">Permissions</span></span>

<span data-ttu-id="e6f10-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="e6f10-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f10-114">Permission type</span></span>             |                                           <span data-ttu-id="e6f10-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6f10-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e6f10-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6f10-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6f10-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f10-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="e6f10-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6f10-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f10-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f10-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="e6f10-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6f10-120">Application</span></span>                            | <span data-ttu-id="e6f10-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f10-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="e6f10-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6f10-122">HTTP Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6f10-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f10-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}
```
# <a name="c"></a>[<span data-ttu-id="e6f10-124">C#</span><span class="sxs-lookup"><span data-stu-id="e6f10-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6f10-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6f10-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6f10-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6f10-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6f10-127">Java</span><span class="sxs-lookup"><span data-stu-id="e6f10-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="e6f10-128">Имена специальных папок</span><span class="sxs-lookup"><span data-stu-id="e6f10-128">Special folder names</span></span>

<span data-ttu-id="e6f10-129">Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e6f10-129">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="e6f10-130">Имя</span><span class="sxs-lookup"><span data-stu-id="e6f10-130">Name</span></span>        | <span data-ttu-id="e6f10-131">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="e6f10-131">Folder id</span></span>    | <span data-ttu-id="e6f10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e6f10-132">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="e6f10-133">Документы</span><span class="sxs-lookup"><span data-stu-id="e6f10-133">Documents</span></span>   | `documents`  | <span data-ttu-id="e6f10-134">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="e6f10-134">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="e6f10-135">Фотографии</span><span class="sxs-lookup"><span data-stu-id="e6f10-135">Photos</span></span>      | `photos`     | <span data-ttu-id="e6f10-136">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="e6f10-136">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="e6f10-137">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="e6f10-137">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="e6f10-138">Папка для резервных копий альбома камеры.</span><span class="sxs-lookup"><span data-stu-id="e6f10-138">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="e6f10-139">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="e6f10-139">App Root</span></span>    | `approot`    | <span data-ttu-id="e6f10-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="e6f10-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="e6f10-142">Музыка</span><span class="sxs-lookup"><span data-stu-id="e6f10-142">Music</span></span>       | `music`      | <span data-ttu-id="e6f10-143">Папка "Музыка".</span><span class="sxs-lookup"><span data-stu-id="e6f10-143">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="e6f10-144">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6f10-144">Optional query parameters</span></span>

<span data-ttu-id="e6f10-145">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e6f10-145">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="e6f10-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f10-146">Response</span></span>

<span data-ttu-id="e6f10-147">Этот метод возвращает код ответа `200 OK` и объект [driveItem](../resources/driveitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6f10-147">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="e6f10-148">Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.</span><span class="sxs-lookup"><span data-stu-id="e6f10-148">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="e6f10-149">Получение дочернего элемента специальной папки</span><span class="sxs-lookup"><span data-stu-id="e6f10-149">Get children of a special folder</span></span>

<span data-ttu-id="e6f10-150">Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="e6f10-150">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6f10-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6f10-151">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6f10-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f10-152">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/special/{special-folder-name}/children
```
# <a name="c"></a>[<span data-ttu-id="e6f10-153">C#</span><span class="sxs-lookup"><span data-stu-id="e6f10-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6f10-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6f10-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6f10-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6f10-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6f10-156">Java</span><span class="sxs-lookup"><span data-stu-id="e6f10-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6f10-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f10-157">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="e6f10-158">Примечания</span><span class="sxs-lookup"><span data-stu-id="e6f10-158">Remarks</span></span>

> <span data-ttu-id="e6f10-159">**Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.</span><span class="sxs-lookup"><span data-stu-id="e6f10-159">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="e6f10-160">Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.</span><span class="sxs-lookup"><span data-stu-id="e6f10-160">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
} -->

