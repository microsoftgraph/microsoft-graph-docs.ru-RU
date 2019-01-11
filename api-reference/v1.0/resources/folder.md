---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: fab5db026b47aa84f7d097a19782b70eac6b6064
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821422"
---
# <a name="folder-resource-type"></a><span data-ttu-id="ef634-102">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="ef634-102">Folder resource type</span></span>

<span data-ttu-id="ef634-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="ef634-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef634-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef634-105">JSON representation</span></span>

<span data-ttu-id="ef634-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef634-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ef634-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef634-107">Properties</span></span>

| <span data-ttu-id="ef634-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef634-108">Property</span></span>       | <span data-ttu-id="ef634-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef634-109">Type</span></span>           | <span data-ttu-id="ef634-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef634-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="ef634-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="ef634-111">**childCount**</span></span> | <span data-ttu-id="ef634-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ef634-112">Int32</span></span>          | <span data-ttu-id="ef634-113">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="ef634-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="ef634-114">**view**</span><span class="sxs-lookup"><span data-stu-id="ef634-114">**view**</span></span>       | <span data-ttu-id="ef634-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="ef634-115">[folderView][]</span></span> | <span data-ttu-id="ef634-116">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="ef634-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="ef634-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef634-117">Remarks</span></span> 

<span data-ttu-id="ef634-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="ef634-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
