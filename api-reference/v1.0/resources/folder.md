---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'Ресурс Folder — это единая структура, объединяющая данные элемента, связанные с папками. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4b43c672b297ce50a5a6aa3dbb3f3d83a1d53be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030333"
---
# <a name="folder-resource-type"></a><span data-ttu-id="99d70-103">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="99d70-103">Folder resource type</span></span>

<span data-ttu-id="99d70-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="99d70-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99d70-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99d70-106">JSON representation</span></span>

<span data-ttu-id="99d70-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99d70-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="99d70-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="99d70-108">Properties</span></span>

| <span data-ttu-id="99d70-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="99d70-109">Property</span></span>       | <span data-ttu-id="99d70-110">Тип</span><span class="sxs-lookup"><span data-stu-id="99d70-110">Type</span></span>           | <span data-ttu-id="99d70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99d70-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="99d70-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="99d70-112">**childCount**</span></span> | <span data-ttu-id="99d70-113">Int32</span><span class="sxs-lookup"><span data-stu-id="99d70-113">Int32</span></span>          | <span data-ttu-id="99d70-114">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="99d70-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="99d70-115">**view**</span><span class="sxs-lookup"><span data-stu-id="99d70-115">**view**</span></span>       | <span data-ttu-id="99d70-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="99d70-116">[folderView][]</span></span> | <span data-ttu-id="99d70-117">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="99d70-117">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="99d70-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="99d70-118">Remarks</span></span> 

<span data-ttu-id="99d70-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="99d70-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
