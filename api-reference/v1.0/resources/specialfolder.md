---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
description: Ресурс SpecialFolder группирует элементы данных, связанные со специальной папкой, в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 142a20c9ea18185f5b7564769d545cca46e9c286
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970531"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="6a08d-103">Тип ресурса SpecialFolder</span><span class="sxs-lookup"><span data-stu-id="6a08d-103">SpecialFolder resource type</span></span>

<span data-ttu-id="6a08d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a08d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a08d-105">Ресурс **SpecialFolder** группирует элементы данных, связанные со специальной папкой, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="6a08d-105">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="6a08d-106">Если у элемента **DriveItem** есть аспект **specialFolder**, значение которого не равно null, то элемент представляет специальную (именованную) папку.</span><span class="sxs-lookup"><span data-stu-id="6a08d-106">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="6a08d-107">Прямой доступ к специальным папкам можно получить с помощью [коллекции специальных папок](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6a08d-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="6a08d-p102">Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.</span><span class="sxs-lookup"><span data-stu-id="6a08d-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="6a08d-p103">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="6a08d-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="6a08d-112">**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="6a08d-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a08d-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a08d-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a08d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a08d-114">Properties</span></span>

| <span data-ttu-id="6a08d-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a08d-115">Property</span></span>  | <span data-ttu-id="6a08d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="6a08d-116">Type</span></span>   | <span data-ttu-id="6a08d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6a08d-117">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="6a08d-118">name</span><span class="sxs-lookup"><span data-stu-id="6a08d-118">name</span></span>      | <span data-ttu-id="6a08d-119">string</span><span class="sxs-lookup"><span data-stu-id="6a08d-119">string</span></span> | <span data-ttu-id="6a08d-120">Уникальный идентификатор для этого элемента в коллекции `/drive/special`.</span><span class="sxs-lookup"><span data-stu-id="6a08d-120">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="6a08d-121">Специальные папки</span><span class="sxs-lookup"><span data-stu-id="6a08d-121">Special folders</span></span>

<span data-ttu-id="6a08d-122">Вот специальные папки, доступные в OneDrive персональный и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6a08d-122">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="6a08d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6a08d-123">Name</span></span>        | <span data-ttu-id="6a08d-124">Идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="6a08d-124">Folder id</span></span>    | <span data-ttu-id="6a08d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6a08d-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="6a08d-126">Корневая папка приложения</span><span class="sxs-lookup"><span data-stu-id="6a08d-126">App Root</span></span>    | `approot`    | <span data-ttu-id="6a08d-p104">Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="6a08d-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="6a08d-129">Альбом камеры</span><span class="sxs-lookup"><span data-stu-id="6a08d-129">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="6a08d-p105">Папка для резервных копий "Альбом камеры". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6a08d-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="6a08d-132">Документы</span><span class="sxs-lookup"><span data-stu-id="6a08d-132">Documents</span></span>   | `documents`  | <span data-ttu-id="6a08d-133">Папка "Документы".</span><span class="sxs-lookup"><span data-stu-id="6a08d-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="6a08d-134">Музыка</span><span class="sxs-lookup"><span data-stu-id="6a08d-134">Music</span></span>       | `music`      | <span data-ttu-id="6a08d-p106">Папка "Музыка". Недоступна в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6a08d-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="6a08d-137">Фотографии</span><span class="sxs-lookup"><span data-stu-id="6a08d-137">Photos</span></span>      | `photos`     | <span data-ttu-id="6a08d-138">Папка "Фотографии".</span><span class="sxs-lookup"><span data-stu-id="6a08d-138">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="6a08d-139">Заметки</span><span class="sxs-lookup"><span data-stu-id="6a08d-139">Remarks</span></span> 

<span data-ttu-id="6a08d-140">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6a08d-140">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->

