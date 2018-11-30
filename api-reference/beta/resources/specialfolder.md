---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
ms.openlocfilehash: 2c316119aeac5208a77f00e04fefcdd2a34cdd7d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079815"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="261c4-102">Тип ресурса SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="261c4-102">SpecialFolder resource type</span></span>

> <span data-ttu-id="261c4-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="261c4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="261c4-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="261c4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="261c4-105">Ресурс **SpecialFolder** группирует элементы данных, связанные со специальной папкой, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="261c4-105">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="261c4-106">Если у элемента **DriveItem** есть аспект **specialFolder**, значение которого не равно null, то элемент представляет специальную (именованную) папку.</span><span class="sxs-lookup"><span data-stu-id="261c4-106">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="261c4-107">Прямой доступ к специальным папкам можно получить с помощью [коллекции специальных папок](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="261c4-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="261c4-p103">Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.</span><span class="sxs-lookup"><span data-stu-id="261c4-p103">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="261c4-p104">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="261c4-p104">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="261c4-112">**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="261c4-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="261c4-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="261c4-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="261c4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="261c4-114">Properties</span></span>

| <span data-ttu-id="261c4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="261c4-115">Property</span></span>  | <span data-ttu-id="261c4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="261c4-116">Type</span></span>   | <span data-ttu-id="261c4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="261c4-117">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="261c4-118">name</span><span class="sxs-lookup"><span data-stu-id="261c4-118">name</span></span>      | <span data-ttu-id="261c4-119">строка</span><span class="sxs-lookup"><span data-stu-id="261c4-119">string</span></span> | <span data-ttu-id="261c4-120">Уникальный идентификатор для этого элемента в коллекции `/drive/special`.</span><span class="sxs-lookup"><span data-stu-id="261c4-120">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="261c4-121">Специальные папки</span><span class="sxs-lookup"><span data-stu-id="261c4-121">Special folders</span></span>

<span data-ttu-id="261c4-122">Вот специальные папки, доступные в OneDrive персональный и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="261c4-122">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="261c4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="261c4-123">Name</span></span>        | <span data-ttu-id="261c4-124">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="261c4-124">Folder id</span></span>    | <span data-ttu-id="261c4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="261c4-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="261c4-126">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="261c4-126">App Root</span></span>    | `approot`    | <span data-ttu-id="261c4-p105">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="261c4-p105">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="261c4-129">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="261c4-129">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="261c4-p106">Папка для резервных копий "Альбом камеры". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="261c4-p106">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="261c4-132">Документы</span><span class="sxs-lookup"><span data-stu-id="261c4-132">Documents</span></span>   | `documents`  | <span data-ttu-id="261c4-133">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="261c4-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="261c4-134">Музыка</span><span class="sxs-lookup"><span data-stu-id="261c4-134">Music</span></span>       | `music`      | <span data-ttu-id="261c4-p107">Папка "Музыка". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="261c4-p107">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="261c4-137">Фотографии</span><span class="sxs-lookup"><span data-stu-id="261c4-137">Photos</span></span>      | `photos`     | <span data-ttu-id="261c4-138">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="261c4-138">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="261c4-139">Заметки</span><span class="sxs-lookup"><span data-stu-id="261c4-139">Remarks</span></span> 

<span data-ttu-id="261c4-140">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="261c4-140">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
