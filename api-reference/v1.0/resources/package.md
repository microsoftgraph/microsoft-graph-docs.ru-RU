---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Package
localization_priority: Normal
ms.openlocfilehash: 6f518058c6a68716f482bd9b6a870457de3d71a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866418"
---
# <a name="package-resource-type"></a><span data-ttu-id="cec8e-102">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="cec8e-102">Package resource type</span></span>

<span data-ttu-id="cec8e-103">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="cec8e-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="cec8e-104">Пример пакета — записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="cec8e-104">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="cec8e-105">Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="cec8e-105">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="cec8e-106">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="cec8e-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cec8e-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cec8e-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="cec8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cec8e-108">Properties</span></span>

| <span data-ttu-id="cec8e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cec8e-109">Property Name</span></span> | <span data-ttu-id="cec8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cec8e-110">Type</span></span>   | <span data-ttu-id="cec8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cec8e-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cec8e-112">type</span><span class="sxs-lookup"><span data-stu-id="cec8e-112">type</span></span>          | <span data-ttu-id="cec8e-113">строка</span><span class="sxs-lookup"><span data-stu-id="cec8e-113">string</span></span> | <span data-ttu-id="cec8e-114">String, указывающее тип пакета.</span><span class="sxs-lookup"><span data-stu-id="cec8e-114">A string indicating the type of package.</span></span> <span data-ttu-id="cec8e-115">Во время `oneNote` является единственным в настоящее время определенное значение, должно привести другие типы пакетов возвращаться и соответствующим образом их обработки.</span><span class="sxs-lookup"><span data-stu-id="cec8e-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="cec8e-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="cec8e-116">Remarks</span></span> 

<span data-ttu-id="cec8e-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="cec8e-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
