---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
ms.openlocfilehash: 84e67df8aae6e72363d4ba148e92f9046f41bb29
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="6f503-102">Тип ресурса SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="6f503-102">SpecialFolder resource type</span></span>

<span data-ttu-id="6f503-103">Ресурс **SpecialFolder** группирует элементы данных, связанные со специальной папкой, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="6f503-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="6f503-104">Если у элемента **DriveItem** есть аспект **specialFolder**, значение которого не равно null, то элемент представляет специальную (именованную) папку.</span><span class="sxs-lookup"><span data-stu-id="6f503-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a specail (named) folder. Special folders can be accessed directly via the special folders collection.</span></span>
<span data-ttu-id="6f503-105">Прямой доступ к специальным папкам можно получить с помощью [коллекции специальных папок](../api/drive_get_specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6f503-105">If a DriveItem has a non-null specialFolder facet, the item represents a specail (named) folder. Special folders can be accessed directly via the [special folders collection](../api/drive_get_specialfolder.md).</span></span>

<span data-ttu-id="6f503-p102">Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.</span><span class="sxs-lookup"><span data-stu-id="6f503-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="6f503-p103">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="6f503-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="6f503-110">**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="6f503-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f503-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f503-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6f503-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f503-112">Properties</span></span>

| <span data-ttu-id="6f503-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f503-113">Property</span></span>  | <span data-ttu-id="6f503-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6f503-114">Type</span></span>   | <span data-ttu-id="6f503-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6f503-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="6f503-116">name</span><span class="sxs-lookup"><span data-stu-id="6f503-116">name</span></span>      | <span data-ttu-id="6f503-117">string</span><span class="sxs-lookup"><span data-stu-id="6f503-117">string</span></span> | <span data-ttu-id="6f503-118">Уникальный идентификатор для этого элемента в коллекции `/drive/special`.</span><span class="sxs-lookup"><span data-stu-id="6f503-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="6f503-119">Специальные папки</span><span class="sxs-lookup"><span data-stu-id="6f503-119">Special folders</span></span>

<span data-ttu-id="6f503-120">Вот специальные папки, доступные в OneDrive персональный и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6f503-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="6f503-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6f503-121">Name</span></span>        | <span data-ttu-id="6f503-122">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="6f503-122">Folder id</span></span>    | <span data-ttu-id="6f503-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f503-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="6f503-124">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="6f503-124">App Root</span></span>    | `approot`    | <span data-ttu-id="6f503-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="6f503-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="6f503-127">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="6f503-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="6f503-p105">Папка для резервных копий "Альбом камеры". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6f503-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="6f503-130">Документы</span><span class="sxs-lookup"><span data-stu-id="6f503-130">Documents</span></span>   | `documents`  | <span data-ttu-id="6f503-131">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="6f503-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="6f503-132">Музыка</span><span class="sxs-lookup"><span data-stu-id="6f503-132">Music</span></span>       | `music`      | <span data-ttu-id="6f503-p106">Папка "Музыка". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6f503-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="6f503-135">Фотографии</span><span class="sxs-lookup"><span data-stu-id="6f503-135">Photos</span></span>      | `photos`     | <span data-ttu-id="6f503-136">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="6f503-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="6f503-137">Заметки</span><span class="sxs-lookup"><span data-stu-id="6f503-137">Remarks</span></span> 

<span data-ttu-id="6f503-138">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6f503-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
