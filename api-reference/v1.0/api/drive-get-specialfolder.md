---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение специальных папок
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b28f7044847bc85b9bde1d2a50ab444b64d70dcb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277100"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="1ad68-102">Получение доступа к специальной папке по ее имени</span><span class="sxs-lookup"><span data-stu-id="1ad68-102">Get a special folder by name</span></span>

<span data-ttu-id="1ad68-103">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="1ad68-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="1ad68-p101">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="1ad68-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="1ad68-p102">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="1ad68-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="1ad68-108">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="1ad68-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ad68-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ad68-109">Permissions</span></span>

<span data-ttu-id="1ad68-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ad68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1ad68-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ad68-112">Permission type</span></span>             |                                           <span data-ttu-id="1ad68-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ad68-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1ad68-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ad68-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ad68-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ad68-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="1ad68-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ad68-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ad68-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ad68-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="1ad68-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ad68-118">Application</span></span>                            | <span data-ttu-id="1ad68-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ad68-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="1ad68-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ad68-120">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="1ad68-121">Имена специальных папок</span><span class="sxs-lookup"><span data-stu-id="1ad68-121">Special folder names</span></span>

<span data-ttu-id="1ad68-122">Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1ad68-122">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="1ad68-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1ad68-123">Name</span></span>        | <span data-ttu-id="1ad68-124">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="1ad68-124">Folder id</span></span>    | <span data-ttu-id="1ad68-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1ad68-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="1ad68-126">Документы</span><span class="sxs-lookup"><span data-stu-id="1ad68-126">Documents</span></span>   | `documents`  | <span data-ttu-id="1ad68-127">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="1ad68-127">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="1ad68-128">Фотографии</span><span class="sxs-lookup"><span data-stu-id="1ad68-128">Photos</span></span>      | `photos`     | <span data-ttu-id="1ad68-129">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="1ad68-129">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="1ad68-130">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="1ad68-130">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="1ad68-131">Папка для резервных копий альбома камеры.</span><span class="sxs-lookup"><span data-stu-id="1ad68-131">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="1ad68-132">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="1ad68-132">App Root</span></span>    | `approot`    | <span data-ttu-id="1ad68-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="1ad68-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="1ad68-135">Музыка</span><span class="sxs-lookup"><span data-stu-id="1ad68-135">Music</span></span>       | `music`      | <span data-ttu-id="1ad68-136">Папка "Музыка".</span><span class="sxs-lookup"><span data-stu-id="1ad68-136">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="1ad68-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ad68-137">Optional query parameters</span></span>

<span data-ttu-id="1ad68-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1ad68-138">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="1ad68-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ad68-139">Response</span></span>

<span data-ttu-id="1ad68-140">Этот метод возвращает код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1ad68-140">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="1ad68-141">Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.</span><span class="sxs-lookup"><span data-stu-id="1ad68-141">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ad68-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1ad68-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ad68-143">C#</span><span class="sxs-lookup"><span data-stu-id="1ad68-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-folder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ad68-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ad68-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-folder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1ad68-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1ad68-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-folder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="1ad68-146">Получение дочернего элемента специальной папки</span><span class="sxs-lookup"><span data-stu-id="1ad68-146">Get children of a special folder</span></span>

<span data-ttu-id="1ad68-147">Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="1ad68-147">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="1ad68-148">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ad68-148">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```

### <a name="response"></a><span data-ttu-id="1ad68-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ad68-149">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ad68-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1ad68-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ad68-151">C#</span><span class="sxs-lookup"><span data-stu-id="1ad68-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ad68-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ad68-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1ad68-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1ad68-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="1ad68-154">Замечания</span><span class="sxs-lookup"><span data-stu-id="1ad68-154">Remarks</span></span>

> <span data-ttu-id="1ad68-155">**Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.</span><span class="sxs-lookup"><span data-stu-id="1ad68-155">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="1ad68-156">Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.</span><span class="sxs-lookup"><span data-stu-id="1ad68-156">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
