---
author: JeremyKelley
description: " или коллекция элементов, которые должны рассматриваться как коллекция, а не как отдельные элементы."
ms.date: 09/10/2017
title: Режим
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ae382d1f69a88d814339370264dc5dc7fac9414
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966267"
---
# <a name="package-resource-type"></a><span data-ttu-id="aaabb-103">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="aaabb-103">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaabb-104">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="aaabb-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="aaabb-p101">Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="aaabb-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="aaabb-107">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="aaabb-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaabb-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aaabb-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="aaabb-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aaabb-109">Property Name</span></span> | <span data-ttu-id="aaabb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aaabb-110">Type</span></span>   | <span data-ttu-id="aaabb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aaabb-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aaabb-112">**type**</span><span class="sxs-lookup"><span data-stu-id="aaabb-112">**type**</span></span>      | <span data-ttu-id="aaabb-113">string</span><span class="sxs-lookup"><span data-stu-id="aaabb-113">string</span></span> | <span data-ttu-id="aaabb-p102">Строка, обозначающая тип пакета. Несмотря на то что `oneNote` — единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="aaabb-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="aaabb-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="aaabb-116">Remarks</span></span> 

<span data-ttu-id="aaabb-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="aaabb-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": []
}
-->
