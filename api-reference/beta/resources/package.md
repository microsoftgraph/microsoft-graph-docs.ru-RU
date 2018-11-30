---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Package
ms.openlocfilehash: fe26cf0dc5de00673d5c3c2ae4a90ac80a62897f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081148"
---
# <a name="package-resource-type"></a><span data-ttu-id="1a095-102">Тип ресурса Package</span><span class="sxs-lookup"><span data-stu-id="1a095-102">Package resource type</span></span>

> <span data-ttu-id="1a095-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a095-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a095-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a095-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a095-105">Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.</span><span class="sxs-lookup"><span data-stu-id="1a095-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="1a095-106">Пример пакета — записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="1a095-106">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="1a095-107">Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.</span><span class="sxs-lookup"><span data-stu-id="1a095-107">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="1a095-108">Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.</span><span class="sxs-lookup"><span data-stu-id="1a095-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a095-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a095-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="1a095-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1a095-110">Property Name</span></span> | <span data-ttu-id="1a095-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1a095-111">Type</span></span>   | <span data-ttu-id="1a095-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1a095-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1a095-113">**type**</span><span class="sxs-lookup"><span data-stu-id="1a095-113">**type**</span></span>      | <span data-ttu-id="1a095-114">string</span><span class="sxs-lookup"><span data-stu-id="1a095-114">string</span></span> | <span data-ttu-id="1a095-p103">Строка, обозначающая тип пакета. Несмотря на то что `oneNote` — единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="1a095-p103">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="1a095-117">Заметки</span><span class="sxs-lookup"><span data-stu-id="1a095-117">Remarks</span></span> 

<span data-ttu-id="1a095-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1a095-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation"
} -->
