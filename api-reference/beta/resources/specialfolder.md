---
author: JeremyKelley
description: Группы специальных элементов данных, связанных с папками, в одну структуру.
title: тип ресурса specialFolder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d9552c79588f8533980879c2ed49ed32fdfe7927
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236273"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="66a44-103">тип ресурса specialFolder</span><span class="sxs-lookup"><span data-stu-id="66a44-103">specialFolder resource type</span></span>

<span data-ttu-id="66a44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66a44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66a44-105">Группы специальных элементов данных, связанных с папками, в одну структуру.</span><span class="sxs-lookup"><span data-stu-id="66a44-105">Groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="66a44-106">Если **у driveItem** есть ненулевая грань **specialFolder,** элемент представляет специальную (именовую) папку.</span><span class="sxs-lookup"><span data-stu-id="66a44-106">If a **driveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="66a44-107">Доступ к специальным папкам можно получить через [коллекцию специальных папок](../api/drive-get-specialfolder.md).</span><span class="sxs-lookup"><span data-stu-id="66a44-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="66a44-p102">Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.</span><span class="sxs-lookup"><span data-stu-id="66a44-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="66a44-p103">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="66a44-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]

><span data-ttu-id="66a44-112">**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="66a44-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="properties"></a><span data-ttu-id="66a44-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="66a44-113">Properties</span></span>

| <span data-ttu-id="66a44-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="66a44-114">Property</span></span>  | <span data-ttu-id="66a44-115">Тип</span><span class="sxs-lookup"><span data-stu-id="66a44-115">Type</span></span>   | <span data-ttu-id="66a44-116">Описание</span><span class="sxs-lookup"><span data-stu-id="66a44-116">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="66a44-117">name</span><span class="sxs-lookup"><span data-stu-id="66a44-117">name</span></span>      | <span data-ttu-id="66a44-118">string</span><span class="sxs-lookup"><span data-stu-id="66a44-118">string</span></span> | <span data-ttu-id="66a44-119">Уникальный идентификатор для этого элемента в коллекции `/drive/special`.</span><span class="sxs-lookup"><span data-stu-id="66a44-119">The unique identifier for this item in the `/drive/special` collection</span></span> |


## <a name="json-representation"></a><span data-ttu-id="66a44-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="66a44-120">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="66a44-121">См. также</span><span class="sxs-lookup"><span data-stu-id="66a44-121">See also</span></span> 

<span data-ttu-id="66a44-122">Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="66a44-122">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


