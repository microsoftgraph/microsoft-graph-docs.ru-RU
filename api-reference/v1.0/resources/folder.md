---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 664597297700f7af096ef30cfbd5342a45a6c157
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="folder-resource-type"></a><span data-ttu-id="3b428-102">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="3b428-102">Folder resource type</span></span>

<span data-ttu-id="3b428-103">Ресурс **Folder** группирует данные, связанные с папкой, в элементе в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="3b428-103">The **Folder** resource groups folder-related data on an item into a single structure. DriveItems with a non-null folder facet are containers for other DriveItems.</span></span> 
<span data-ttu-id="3b428-104">Ресурсы [**DriveItem**](driveitem.md), у которых значение аспекта **folder** не равно null, представляют собой контейнеры для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="3b428-104">The Folder resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b428-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3b428-105">JSON representation</span></span>

<span data-ttu-id="3b428-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b428-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3b428-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b428-107">Properties</span></span>

| <span data-ttu-id="3b428-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b428-108">Property</span></span>       | <span data-ttu-id="3b428-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3b428-109">Type</span></span>           | <span data-ttu-id="3b428-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b428-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="3b428-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="3b428-111">**childCount**</span></span> | <span data-ttu-id="3b428-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3b428-112">Int64</span></span>          | <span data-ttu-id="3b428-113">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="3b428-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="3b428-114">**view**</span><span class="sxs-lookup"><span data-stu-id="3b428-114">**view**</span></span>       | <span data-ttu-id="3b428-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="3b428-115">[folderView facet][]</span></span> | <span data-ttu-id="3b428-116">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="3b428-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="3b428-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b428-117">Remarks</span></span> 

<span data-ttu-id="3b428-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="3b428-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
