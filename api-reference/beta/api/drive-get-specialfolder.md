---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение специальных папок
localization_priority: Normal
ms.openlocfilehash: c63f3ae585db0aff812e16eb9f125d19e77a806c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887957"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="fa858-102">Получение специальной папки по ее имени</span><span class="sxs-lookup"><span data-stu-id="fa858-102">Get a special folder by name</span></span>

> <span data-ttu-id="fa858-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa858-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa858-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa858-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa858-105">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="fa858-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="fa858-p102">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="fa858-p102">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="fa858-p103">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="fa858-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="fa858-110">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="fa858-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa858-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa858-111">Permissions</span></span>

<span data-ttu-id="fa858-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa858-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="fa858-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa858-114">Permission type</span></span>             |                                           <span data-ttu-id="fa858-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa858-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fa858-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa858-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa858-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa858-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="fa858-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa858-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa858-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa858-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="fa858-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa858-120">Application</span></span>                            | <span data-ttu-id="fa858-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa858-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="fa858-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa858-122">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="fa858-123">Имена специальных папок</span><span class="sxs-lookup"><span data-stu-id="fa858-123">Special folder names</span></span>

<span data-ttu-id="fa858-124">Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fa858-124">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="fa858-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fa858-125">Name</span></span>        | <span data-ttu-id="fa858-126">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="fa858-126">Folder id</span></span>    | <span data-ttu-id="fa858-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fa858-127">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="fa858-128">Документы</span><span class="sxs-lookup"><span data-stu-id="fa858-128">Documents</span></span>   | `documents`  | <span data-ttu-id="fa858-129">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="fa858-129">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="fa858-130">Фотографии</span><span class="sxs-lookup"><span data-stu-id="fa858-130">Photos</span></span>      | `photos`     | <span data-ttu-id="fa858-131">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="fa858-131">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="fa858-132">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="fa858-132">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="fa858-133">Папка для резервных копий альбома камеры.</span><span class="sxs-lookup"><span data-stu-id="fa858-133">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="fa858-134">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="fa858-134">App Root</span></span>    | `approot`    | <span data-ttu-id="fa858-p105">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="fa858-p105">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="fa858-137">Музыка</span><span class="sxs-lookup"><span data-stu-id="fa858-137">Music</span></span>       | `music`      | <span data-ttu-id="fa858-138">Папка "Музыка".</span><span class="sxs-lookup"><span data-stu-id="fa858-138">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="fa858-139">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa858-139">Optional query parameters</span></span>

<span data-ttu-id="fa858-140">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fa858-140">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="fa858-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa858-141">Response</span></span>

<span data-ttu-id="fa858-142">Этот метод возвращает код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa858-142">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="fa858-143">Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.</span><span class="sxs-lookup"><span data-stu-id="fa858-143">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="fa858-144">Получение дочернего элемента специальной папки</span><span class="sxs-lookup"><span data-stu-id="fa858-144">Get children of a special folder</span></span>

<span data-ttu-id="fa858-145">Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="fa858-145">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="fa858-146">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa858-146">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="response"></a><span data-ttu-id="fa858-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa858-147">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="fa858-148">Примечания</span><span class="sxs-lookup"><span data-stu-id="fa858-148">Remarks</span></span>

> <span data-ttu-id="fa858-149">**Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.</span><span class="sxs-lookup"><span data-stu-id="fa858-149">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="fa858-150">Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.</span><span class="sxs-lookup"><span data-stu-id="fa858-150">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
