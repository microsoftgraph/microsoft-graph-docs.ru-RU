---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: 5b187b1b4ff7183739ed734256a2d4c9e9fa9af6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512187"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="28623-102">Тип ресурса SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="28623-102">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28623-103">Ресурс **SpecialFolder** группирует элементы данных, связанные со специальной папкой, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="28623-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="28623-104">Если у элемента **DriveItem** есть аспект **specialFolder**, значение которого не равно null, то элемент представляет специальную (именованную) папку.</span><span class="sxs-lookup"><span data-stu-id="28623-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="28623-105">Прямой доступ к специальным папкам можно получить с помощью [коллекции специальных папок](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="28623-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="28623-p102">Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.</span><span class="sxs-lookup"><span data-stu-id="28623-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="28623-p103">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="28623-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="28623-110">**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="28623-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28623-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28623-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="28623-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="28623-112">Properties</span></span>

| <span data-ttu-id="28623-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="28623-113">Property</span></span>  | <span data-ttu-id="28623-114">Тип</span><span class="sxs-lookup"><span data-stu-id="28623-114">Type</span></span>   | <span data-ttu-id="28623-115">Описание</span><span class="sxs-lookup"><span data-stu-id="28623-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="28623-116">name</span><span class="sxs-lookup"><span data-stu-id="28623-116">name</span></span>      | <span data-ttu-id="28623-117">string</span><span class="sxs-lookup"><span data-stu-id="28623-117">string</span></span> | <span data-ttu-id="28623-118">Уникальный идентификатор для этого элемента в коллекции `/drive/special`.</span><span class="sxs-lookup"><span data-stu-id="28623-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="28623-119">Специальные папки</span><span class="sxs-lookup"><span data-stu-id="28623-119">Special folders</span></span>

<span data-ttu-id="28623-120">Вот специальные папки, доступные в OneDrive персональный и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="28623-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="28623-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28623-121">Name</span></span>        | <span data-ttu-id="28623-122">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="28623-122">Folder id</span></span>    | <span data-ttu-id="28623-123">Описание</span><span class="sxs-lookup"><span data-stu-id="28623-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="28623-124">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="28623-124">App Root</span></span>    | `approot`    | <span data-ttu-id="28623-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="28623-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="28623-127">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="28623-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="28623-p105">Папка для резервных копий "Альбом камеры". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="28623-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="28623-130">Документы</span><span class="sxs-lookup"><span data-stu-id="28623-130">Documents</span></span>   | `documents`  | <span data-ttu-id="28623-131">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="28623-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="28623-132">Музыка</span><span class="sxs-lookup"><span data-stu-id="28623-132">Music</span></span>       | `music`      | <span data-ttu-id="28623-p106">Папка "Музыка". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="28623-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="28623-135">Фотографии</span><span class="sxs-lookup"><span data-stu-id="28623-135">Photos</span></span>      | `photos`     | <span data-ttu-id="28623-136">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="28623-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="28623-137">Заметки</span><span class="sxs-lookup"><span data-stu-id="28623-137">Remarks</span></span> 

<span data-ttu-id="28623-138">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="28623-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/specialfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
