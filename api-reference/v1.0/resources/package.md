---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Пакет
localization_priority: Normal
ms.openlocfilehash: c64dfce910456ef9b9415e3332c099d7814a71f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462531"
---
# <a name="package-resource-type"></a><span data-ttu-id="c5038-102">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="c5038-102">Package resource type</span></span>

<span data-ttu-id="c5038-103">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="c5038-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="c5038-p101">Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="c5038-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="c5038-106">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="c5038-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5038-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5038-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="c5038-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5038-108">Properties</span></span>

| <span data-ttu-id="c5038-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c5038-109">Property Name</span></span> | <span data-ttu-id="c5038-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c5038-110">Type</span></span>   | <span data-ttu-id="c5038-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5038-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c5038-112">type</span><span class="sxs-lookup"><span data-stu-id="c5038-112">type</span></span>          | <span data-ttu-id="c5038-113">string</span><span class="sxs-lookup"><span data-stu-id="c5038-113">string</span></span> | <span data-ttu-id="c5038-114">Строка, указывающая тип пакета.</span><span class="sxs-lookup"><span data-stu-id="c5038-114">A string indicating the type of package.</span></span> <span data-ttu-id="c5038-115">Несмотря на то что `oneNote`— единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="c5038-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c5038-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="c5038-116">Remarks</span></span> 

<span data-ttu-id="c5038-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c5038-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
