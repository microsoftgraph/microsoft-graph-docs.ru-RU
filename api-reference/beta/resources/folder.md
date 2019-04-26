---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: 77c13d980590e908de5c7f0a8a7cbf67d1cf031e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340254"
---
# <a name="folder-resource-type"></a><span data-ttu-id="ebb08-102">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="ebb08-102">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebb08-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="ebb08-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb08-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebb08-105">JSON representation</span></span>

<span data-ttu-id="ebb08-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebb08-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ebb08-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebb08-107">Properties</span></span>

| <span data-ttu-id="ebb08-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebb08-108">Property</span></span>       | <span data-ttu-id="ebb08-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ebb08-109">Type</span></span>           | <span data-ttu-id="ebb08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb08-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="ebb08-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="ebb08-111">**childCount**</span></span> | <span data-ttu-id="ebb08-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ebb08-112">Int64</span></span>          | <span data-ttu-id="ebb08-113">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="ebb08-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="ebb08-114">**view**</span><span class="sxs-lookup"><span data-stu-id="ebb08-114">**view**</span></span>       | <span data-ttu-id="ebb08-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="ebb08-115">[folderView][]</span></span> | <span data-ttu-id="ebb08-116">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="ebb08-116">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="ebb08-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="ebb08-117">Remarks</span></span> 

<span data-ttu-id="ebb08-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="ebb08-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
