---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение специальных папок
localization_priority: Normal
ms.prod: sharepoint
description: Используйте специальную коллекцию для доступа к специальной папке по имени.
doc_type: apiPageType
ms.openlocfilehash: 662ee2f2dae0e3f8684d76fbc18b3315a80133dd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375200"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="6d35f-103">Получение доступа к специальной папке по ее имени</span><span class="sxs-lookup"><span data-stu-id="6d35f-103">Get a special folder by name</span></span>

<span data-ttu-id="6d35f-104">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="6d35f-104">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="6d35f-p101">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="6d35f-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="6d35f-p102">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="6d35f-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="6d35f-109">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="6d35f-109">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d35f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d35f-110">Permissions</span></span>

<span data-ttu-id="6d35f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d35f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6d35f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d35f-113">Permission type</span></span>             |                                           <span data-ttu-id="6d35f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d35f-114">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6d35f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d35f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d35f-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d35f-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="6d35f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d35f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d35f-118">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d35f-118">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="6d35f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d35f-119">Application</span></span>                            | <span data-ttu-id="6d35f-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d35f-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="6d35f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d35f-121">HTTP Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d35f-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d35f-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d35f-123">C#</span><span class="sxs-lookup"><span data-stu-id="6d35f-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d35f-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d35f-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d35f-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6d35f-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d35f-126">Java</span><span class="sxs-lookup"><span data-stu-id="6d35f-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="6d35f-127">Имена специальных папок</span><span class="sxs-lookup"><span data-stu-id="6d35f-127">Special folder names</span></span>

<span data-ttu-id="6d35f-128">Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6d35f-128">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="6d35f-129">Имя</span><span class="sxs-lookup"><span data-stu-id="6d35f-129">Name</span></span>        | <span data-ttu-id="6d35f-130">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="6d35f-130">Folder id</span></span>    | <span data-ttu-id="6d35f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d35f-131">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="6d35f-132">Документы</span><span class="sxs-lookup"><span data-stu-id="6d35f-132">Documents</span></span>   | `documents`  | <span data-ttu-id="6d35f-133">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="6d35f-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="6d35f-134">Фотографии</span><span class="sxs-lookup"><span data-stu-id="6d35f-134">Photos</span></span>      | `photos`     | <span data-ttu-id="6d35f-135">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="6d35f-135">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="6d35f-136">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="6d35f-136">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="6d35f-137">Папка для резервных копий альбома камеры.</span><span class="sxs-lookup"><span data-stu-id="6d35f-137">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="6d35f-138">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="6d35f-138">App Root</span></span>    | `approot`    | <span data-ttu-id="6d35f-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="6d35f-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="6d35f-141">Музыка</span><span class="sxs-lookup"><span data-stu-id="6d35f-141">Music</span></span>       | `music`      | <span data-ttu-id="6d35f-142">Папка "Музыка".</span><span class="sxs-lookup"><span data-stu-id="6d35f-142">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="6d35f-143">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d35f-143">Optional query parameters</span></span>

<span data-ttu-id="6d35f-144">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6d35f-144">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="6d35f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d35f-145">Response</span></span>

<span data-ttu-id="6d35f-146">Этот метод возвращает код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d35f-146">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="6d35f-147">Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.</span><span class="sxs-lookup"><span data-stu-id="6d35f-147">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="6d35f-148">Получение дочернего элемента специальной папки</span><span class="sxs-lookup"><span data-stu-id="6d35f-148">Get children of a special folder</span></span>

<span data-ttu-id="6d35f-149">Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="6d35f-149">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d35f-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d35f-150">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d35f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d35f-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d35f-152">C#</span><span class="sxs-lookup"><span data-stu-id="6d35f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d35f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d35f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d35f-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6d35f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d35f-155">Java</span><span class="sxs-lookup"><span data-stu-id="6d35f-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d35f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d35f-156">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="6d35f-157">Примечания</span><span class="sxs-lookup"><span data-stu-id="6d35f-157">Remarks</span></span>

> <span data-ttu-id="6d35f-158">**Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.</span><span class="sxs-lookup"><span data-stu-id="6d35f-158">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="6d35f-159">Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.</span><span class="sxs-lookup"><span data-stu-id="6d35f-159">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
} -->
