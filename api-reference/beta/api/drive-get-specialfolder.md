---
author: JeremyKelley
description: Используйте специальную коллекцию для доступа к специальной папке по имени.
ms.date: 09/10/2017
title: Получение специальных папок
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 04f34a560fc72f47a0797c02f02e36e7e91a9838
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433316"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="5398d-103">Получение доступа к специальной папке по ее имени</span><span class="sxs-lookup"><span data-stu-id="5398d-103">Get a special folder by name</span></span>

<span data-ttu-id="5398d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5398d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5398d-105">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="5398d-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="5398d-p101">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="5398d-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="5398d-p102">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="5398d-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="5398d-110">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="5398d-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5398d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5398d-111">Permissions</span></span>

<span data-ttu-id="5398d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5398d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="5398d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5398d-114">Permission type</span></span>             |                                           <span data-ttu-id="5398d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5398d-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5398d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5398d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5398d-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5398d-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="5398d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5398d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5398d-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5398d-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="5398d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5398d-120">Application</span></span>                            | <span data-ttu-id="5398d-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5398d-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="5398d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5398d-122">HTTP Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5398d-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="5398d-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}
```
# <a name="c"></a>[<span data-ttu-id="5398d-124">C#</span><span class="sxs-lookup"><span data-stu-id="5398d-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5398d-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5398d-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5398d-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5398d-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="5398d-127">Имена специальных папок</span><span class="sxs-lookup"><span data-stu-id="5398d-127">Special folder names</span></span>

<span data-ttu-id="5398d-128">Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5398d-128">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="5398d-129">Имя</span><span class="sxs-lookup"><span data-stu-id="5398d-129">Name</span></span>        | <span data-ttu-id="5398d-130">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="5398d-130">Folder id</span></span>    | <span data-ttu-id="5398d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5398d-131">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="5398d-132">Документы</span><span class="sxs-lookup"><span data-stu-id="5398d-132">Documents</span></span>   | `documents`  | <span data-ttu-id="5398d-133">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="5398d-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="5398d-134">Фотографии</span><span class="sxs-lookup"><span data-stu-id="5398d-134">Photos</span></span>      | `photos`     | <span data-ttu-id="5398d-135">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="5398d-135">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="5398d-136">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="5398d-136">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="5398d-137">Папка для резервных копий альбома камеры.</span><span class="sxs-lookup"><span data-stu-id="5398d-137">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="5398d-138">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="5398d-138">App Root</span></span>    | `approot`    | <span data-ttu-id="5398d-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="5398d-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="5398d-141">Музыка</span><span class="sxs-lookup"><span data-stu-id="5398d-141">Music</span></span>       | `music`      | <span data-ttu-id="5398d-142">Папка "Музыка".</span><span class="sxs-lookup"><span data-stu-id="5398d-142">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="5398d-143">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5398d-143">Optional query parameters</span></span>

<span data-ttu-id="5398d-144">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5398d-144">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="5398d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5398d-145">Response</span></span>

<span data-ttu-id="5398d-146">Этот метод возвращает код ответа `200 OK` и объект [driveItem](../resources/driveitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5398d-146">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="5398d-147">Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.</span><span class="sxs-lookup"><span data-stu-id="5398d-147">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="5398d-148">Получение дочернего элемента специальной папки</span><span class="sxs-lookup"><span data-stu-id="5398d-148">Get children of a special folder</span></span>

<span data-ttu-id="5398d-149">Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="5398d-149">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="5398d-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5398d-150">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="5398d-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5398d-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}/children
```
# <a name="c"></a>[<span data-ttu-id="5398d-152">C#</span><span class="sxs-lookup"><span data-stu-id="5398d-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5398d-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5398d-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5398d-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5398d-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5398d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5398d-155">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="5398d-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="5398d-156">Remarks</span></span>

> <span data-ttu-id="5398d-157">**Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.</span><span class="sxs-lookup"><span data-stu-id="5398d-157">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="5398d-158">Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.</span><span class="sxs-lookup"><span data-stu-id="5398d-158">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
}
-->
