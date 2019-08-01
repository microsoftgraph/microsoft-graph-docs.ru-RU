---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Режим
localization_priority: Normal
description: " или коллекция элементов, которые должны рассматриваться как коллекция, а не как отдельные элементы."
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8eff13e0cfdc6b355cc289833e7b3050ded2641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035667"
---
# <a name="package-resource-type"></a><span data-ttu-id="e2e5e-103">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="e2e5e-103">Package resource type</span></span>

<span data-ttu-id="e2e5e-104">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="e2e5e-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="e2e5e-p101">Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="e2e5e-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="e2e5e-107">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="e2e5e-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2e5e-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2e5e-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="e2e5e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2e5e-109">Properties</span></span>

| <span data-ttu-id="e2e5e-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e2e5e-110">Property Name</span></span> | <span data-ttu-id="e2e5e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e2e5e-111">Type</span></span>   | <span data-ttu-id="e2e5e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e5e-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e2e5e-113">type</span><span class="sxs-lookup"><span data-stu-id="e2e5e-113">type</span></span>          | <span data-ttu-id="e2e5e-114">string</span><span class="sxs-lookup"><span data-stu-id="e2e5e-114">string</span></span> | <span data-ttu-id="e2e5e-115">Строка, указывающая тип пакета.</span><span class="sxs-lookup"><span data-stu-id="e2e5e-115">A string indicating the type of package.</span></span> <span data-ttu-id="e2e5e-116">Несмотря на то что `oneNote`— единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="e2e5e-116">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e2e5e-117">Заметки</span><span class="sxs-lookup"><span data-stu-id="e2e5e-117">Remarks</span></span> 

<span data-ttu-id="e2e5e-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e2e5e-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
