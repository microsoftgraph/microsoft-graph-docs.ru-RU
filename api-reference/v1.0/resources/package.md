---
author: JeremyKelley
ms.date: 09/10/2017
title: Пакет
localization_priority: Normal
description: " или коллекция элементов, которые должны рассматриваться как коллекция, а не как отдельные элементы."
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e248c74add209690dbd7c3cc11d8056c5ca30dcc
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239816"
---
# <a name="package-resource-type"></a><span data-ttu-id="9ae4a-103">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="9ae4a-103">Package resource type</span></span>

<span data-ttu-id="9ae4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ae4a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ae4a-105">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="9ae4a-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="9ae4a-p101">Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="9ae4a-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="9ae4a-108">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="9ae4a-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ae4a-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ae4a-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="9ae4a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ae4a-110">Properties</span></span>

| <span data-ttu-id="9ae4a-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9ae4a-111">Property Name</span></span> | <span data-ttu-id="9ae4a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9ae4a-112">Type</span></span>   | <span data-ttu-id="9ae4a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9ae4a-113">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9ae4a-114">type</span><span class="sxs-lookup"><span data-stu-id="9ae4a-114">type</span></span>          | <span data-ttu-id="9ae4a-115">string</span><span class="sxs-lookup"><span data-stu-id="9ae4a-115">string</span></span> | <span data-ttu-id="9ae4a-116">Строка, указывающая тип пакета.</span><span class="sxs-lookup"><span data-stu-id="9ae4a-116">A string indicating the type of package.</span></span> <span data-ttu-id="9ae4a-117">Несмотря на то что `oneNote`— единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="9ae4a-117">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9ae4a-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="9ae4a-118">Remarks</span></span> 

<span data-ttu-id="9ae4a-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9ae4a-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

